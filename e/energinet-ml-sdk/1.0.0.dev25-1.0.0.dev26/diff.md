# Comparing `tmp/energinet-ml-sdk-1.0.0.dev25.tar.gz` & `tmp/energinet-ml-sdk-1.0.0.dev26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energinet-ml-sdk-1.0.0.dev25.tar", last modified: Mon May 22 07:50:30 2023, max compression
+gzip compressed data, was "energinet-ml-sdk-1.0.0.dev26.tar", last modified: Tue Jun 13 13:59:34 2023, max compression
```

## Comparing `energinet-ml-sdk-1.0.0.dev25.tar` & `energinet-ml-sdk-1.0.0.dev26.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/
--rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1733 2023-05-22 07:50:15.862798 energinet-ml-sdk-1.0.0.dev25/README
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/
--rw-r--r--   0 vsts      (1001) docker     (123)      210 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13179 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/backend.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8140 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/datasets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4352 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/interactive.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2130 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/submitting.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6853 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/azure/training.py
--rw-r--r--   0 vsts      (1001) docker     (123)      190 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/backend.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      581 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/files.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2965 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/init.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3133 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/release.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5525 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/submit.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5250 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/train.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/
--rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7294 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11202 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/projects.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/verify.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/core/
--rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4552 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/backend.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4381 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/configurable.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3006 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/files.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3760 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27442 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2555 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1871 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/requirements.py
--rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/submitting.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9048 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/templates.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3293 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/core/training.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/
--rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/COMMAND_NAME
--rw-r--r--   0 vsts      (1001) docker     (123)       17 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/PACKAGE_NAME
--rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-05-22 07:50:30.098775 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/PACKAGE_VERSION
--rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/meta/PYTHON_VERSION
--rw-r--r--   0 vsts      (1001) docker     (123)     2793 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/settings.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/static/
--rw-r--r--   0 vsts      (1001) docker     (123)      492 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/Dockerfile
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      147 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1728 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4481 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (123)      715 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/constants.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.662775 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      515 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8099 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/backend_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4350 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/datasets_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      675 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/training_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      899 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/files_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3739 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/init_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/release_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9074 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/submit_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3566 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/train_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.870798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2310 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/init_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4922 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/decorators_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7759 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/projects_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:30.666775 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2197 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/backend_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1126 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/configurable_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/files_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/logger_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14679 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/model_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2874 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/project_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2378 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/requirements_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-05-22 07:50:15.874798 energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/submitting_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/
+-rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1733 2023-06-13 13:59:25.465278 energinet-ml-sdk-1.0.0.dev26/README
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/
+-rw-r--r--   0 vsts      (1001) docker     (123)      210 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13203 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8140 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/datasets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4352 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2130 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7370 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/training.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      190 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/backend.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      581 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2965 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/init.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3133 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/release.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5525 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/submit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5415 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/train.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7294 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11202 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/projects.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/verify.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4552 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4381 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/configurable.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3006 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4609 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27442 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2555 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1871 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/requirements.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9048 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/templates.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3293 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/training.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/
+-rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/COMMAND_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       17 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/PACKAGE_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-06-13 13:59:34.401189 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/PACKAGE_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/PYTHON_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)     2793 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/settings.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)      492 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/Dockerfile
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      147 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1728 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4481 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      715 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/constants.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      515 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8099 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4350 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/datasets_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      675 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/training_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      899 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3739 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/init_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/release_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9074 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/submit_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3566 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/train_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2310 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/init_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4922 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/decorators_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7759 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/projects_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2197 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1126 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/configurable_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/logger_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14679 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/model_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2874 2023-06-13 13:59:25.477278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/project_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2378 2023-06-13 13:59:25.477278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/requirements_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-06-13 13:59:25.477278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/submitting_test.py
```

### Comparing `energinet-ml-sdk-1.0.0.dev25/PKG-INFO` & `energinet-ml-sdk-1.0.0.dev26/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energinet-ml-sdk
-Version: 1.0.0.dev25
+Version: 1.0.0.dev26
 Summary: Energinet Machine Learning
 Home-page: UNKNOWN
 Author: Koncern Digitalisering Advanced Analytics Team
 Author-email: mny@energinet.dk, xjakk@energinet.dk
 License: Apache Software License 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `energinet-ml-sdk-1.0.0.dev25/README` & `energinet-ml-sdk-1.0.0.dev26/README`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/backend.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,25 +252,25 @@
             )
         except azureml._common.exceptions.AzureMLException as e:
             raise self.parse_azureml_exception(e)
 
     # -- Contexts ------------------------------------------------------------
 
     def get_local_training_context(
-        self, force_download: bool
+        self, force_download: bool, dry_run: bool
     ) -> AzureLocalTrainingContext:
         """[summary]
 
         Args:
             force_download (bool): [description]
 
         Returns:
             AzureLocalTrainingContext: [description]
         """
-        return AzureLocalTrainingContext(self, force_download)
+        return AzureLocalTrainingContext(self, force_download, dry_run)
 
     def get_cloud_training_context(self) -> AzureCloudTrainingContext:
         """[summary]
 
         Returns:
             AzureCloudTrainingContext: [description]
         """
```

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/datasets.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/datasets.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/interactive.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/interactive.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/logger.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/logger.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/submitting.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/submitting.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/azure/training.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """[summary]
 """
 import json
 import os
 from typing import TYPE_CHECKING, Any, Dict, List
+from unittest import mock
 
 import azureml
 from azureml.core import Experiment, Run
 
 from energinetml.azure.datasets import (
     DownloadedAzureMLDataStore,
     MountedAzureMLDataStore,
 )
 from energinetml.azure.logger import AzureMlLogger
-from energinetml.core.logger import ConsoleLogger
+from energinetml.core.logger import ConsoleLogger, EchoLogger
 from energinetml.core.training import AbstractTrainingContext
 from energinetml.settings import DEFAULT_RELATIVE_ARTIFACT_PATH
 
 if TYPE_CHECKING:
     from energinetml.azure.backend import AzureBackend
     from energinetml.core.model import Model, TrainedModel
 
@@ -74,23 +75,24 @@
         except azureml._common.exceptions.AzureMLException as ex:
             raise self.backend.parse_azureml_exception(ex)
 
 
 class AzureLocalTrainingContext(AzureTrainingContext):
     """[summary]"""
 
-    def __init__(self, backend: "AzureBackend", force_download: bool):
+    def __init__(self, backend: "AzureBackend", force_download: bool, dry_run: bool):
         """[summary]
 
         Args:
             backend (AzureBackend): [description]
             force_download (bool): [description]
         """
         self.backend = backend
         self.force_download = force_download
+        self.dry_run = dry_run
         self.az_run = None
 
     def train_model(
         self, model: "Model", tags: Dict[str, Any], **kwargs
     ) -> "TrainedModel":
         """[summary]
 
@@ -118,33 +120,44 @@
         )
 
         with model.temporary_folder() as temp_path:
             # The "outputs" parameter is provided here with a non-existing
             # folder path to avoid having azureml upload files. We will do
             # this manually somewhere else.
 
-            try:
-                self.az_run = az_experiment.start_logging(
-                    snapshot_directory=temp_path,
-                    outputs=os.path.join(temp_path, "a-folder-that-does-not-exists"),
-                )
-            except azureml._common.exceptions.AzureMLException as ex:
-                raise self.backend.parse_azureml_exception(ex)
-
-            self.az_run.set_tags(tags)
-            try:
-                return model.train(
-                    datasets=datasets, logger=AzureMlLogger(self.az_run), **kwargs
-                )
-            finally:
+            if self.dry_run:
                 try:
-                    self.az_run.complete()
+                    return model.train(
+                        datasets=datasets, logger=EchoLogger(), **kwargs
+                    )
+                except Exception as ex:
+                    raise self.backend.parse_azureml_exception(ex)
+            else:
+                try:
+                    self.az_run = az_experiment.start_logging(
+                        snapshot_directory=temp_path,
+                        outputs=os.path.join(
+                            temp_path, "a-folder-that-does-not-exists"
+                        ),
+                    )
                 except azureml._common.exceptions.AzureMLException as ex:
                     raise self.backend.parse_azureml_exception(ex)
 
+                self.az_run.set_tags(tags)
+
+                try:
+                    return model.train(
+                        datasets=datasets, logger=AzureMlLogger(self.az_run), **kwargs
+                    )
+                finally:
+                    try:
+                        self.az_run.complete()
+                    except azureml._common.exceptions.AzureMLException as ex:
+                        raise self.backend.parse_azureml_exception(ex)
+
     def get_parameters(self, model: "Model") -> Dict:
         """[summary]
 
         Args:
             model (Model): [description]
 
         Returns:
```

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/__init__.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/__init__.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/__init__.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/init.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/init.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/release.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/release.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/submit.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/submit.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/model/train.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,28 @@
     "-f",
     "force_download",
     default=False,
     is_flag=True,
     help="Force download of datasets (ignore locally cached files)",
 )
 @click.option("--seed", "-s", required=False, default=None, type=str, help="Seed value")
+@click.option(
+    "--dry-run",
+    "-d",
+    "dry_run",
+    default=False,
+    is_flag=True,
+    help="Run training without tracking",
+)
 def train(
     parameters: List[str],
     cloud_mode: bool,
     force_download: bool,
     seed: Union[int, str],
+    dry_run: bool,
     model: Model,
 ):
     """Train a model locally"""
 
     try:
         stdout_console_logger = ConsoleLogger(name="stdout", console=sys.stdout)
         sys.stdout = stdout_console_logger
@@ -56,15 +65,15 @@
         # -- Training context ----------------------------------------------------
 
         if cloud_mode:
             # Training is running in the cloud
             context = backend.get_cloud_training_context()
         else:
             # Training is running locally
-            context = backend.get_local_training_context(force_download)
+            context = backend.get_local_training_context(force_download, dry_run)
 
         # -- Train Parameters ----------------------------------------------------
 
         params = {}
         params.update(context.get_parameters(model))
         params.update(dict(param.split(":") for param in parameters))
         params["seed"] = seed if seed is not None else model.generate_seed()
@@ -119,34 +128,34 @@
         # -- Dump output to disk -------------------------------------------------
 
         print(f"Dumping trained model to: {model.trained_model_path}")
 
         trained_model.params.update(params)
         model.dump(model.trained_model_path, trained_model)
 
-        meta_data = {"module_name": model.module_name, "run_id": context.az_run.id}
+        meta_data = {"module_name": model.module_name}
 
         if context.az_run:
             workspace = context.az_run.experiment.workspace
             meta_data["subscription_id"] = workspace.subscription_id
             meta_data["resource_group"] = workspace.resource_group
             meta_data["workspace_name"] = workspace.name
             meta_data["run_id"] = context.az_run.id
             meta_data["portal_url"] = context.get_portal_url()
 
-        context.save_meta_data(
-            meta_data, os.path.join(model.artifact_path, model._META_FILE_NAME)
-        )
+            context.save_meta_data(
+                meta_data, os.path.join(model.artifact_path, model._META_FILE_NAME)
+            )
 
-        # -- Upload output files -------------------------------------------------
+            # -- Upload output files -------------------------------------------------
 
-        print("Uploading output files...")
+            print("Uploading output files...")
 
-        with click_spinner.spinner():
-            context.save_artifacts(model)
+            with click_spinner.spinner():
+                context.save_artifacts(model)
 
     except Exception:
         raise
     finally:
         if context.az_run:
             # -- Print portal link ---------------------------------------------------
             print(f"Portal link: {context.get_portal_url()}")
```

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/project/init.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/init.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/decorators.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/projects.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/projects.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/cli/utils/verify.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/verify.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/backend.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/backend.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/configurable.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/configurable.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/files.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/files.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/logger.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -135,7 +135,44 @@
             name (str): [description]
             df (pd.DataFrame): [description]
 
         Raises:
             NotImplementedError: [description]
         """
         raise NotImplementedError
+
+
+class EchoLogger(MetricsLogger):
+    def echo(self, s: str) -> None:
+        """[summary]
+
+        Args:
+            s (str): [description]
+        """
+        print(s)
+
+    def log(self, name: str, value: Any) -> None:
+        """[summary]
+
+        Args:
+            name (str): [description]
+            value (Any): [description]
+        """
+        self.echo(f"LOG: {name} = {value}")
+
+    def tag(self, key: str, value: str) -> None:
+        """[summary]
+
+        Args:
+            key (str): [description]
+            value (str): [description]
+        """
+        self.echo(f"TAG: {key} = {value}")
+
+    def dataframe(self, name: str, df: pd.DataFrame) -> None:
+        """[summary]
+
+        Args:
+            name (str): [description]
+            df (pd.DataFrame): [description]
+        """
+        self.echo(f"DATAFRAME: {name} = {df}")
```

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/model.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/model.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/project.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/project.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/requirements.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/requirements.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/submitting.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/submitting.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/templates.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/templates.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/core/training.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/core/training.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/settings.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/settings.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/energinetml/static/model_template/model.py` & `energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/model.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/setup.py` & `energinet-ml-sdk-1.0.0.dev26/setup.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/conftest.py` & `energinet-ml-sdk-1.0.0.dev26/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/constants.py` & `energinet-ml-sdk-1.0.0.dev26/tests/constants.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/smoketest/ml_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/smoketest/webapp_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/backend_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/backend_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/datasets_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/datasets_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/azure_/training_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/training_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/files_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/files_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/init_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/init_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/submit_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/submit_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/model/train_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/train_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/project/init_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/init_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/decorators_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/decorators_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/cli/utils/projects_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/projects_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/backend_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/backend_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/configurable_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/configurable_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/files_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/files_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/logger_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/logger_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/model_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/model_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/project_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/project_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/requirements_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/requirements_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev25/tests/unittests/core/submitting_test.py` & `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/submitting_test.py`

 * *Files identical despite different names*

