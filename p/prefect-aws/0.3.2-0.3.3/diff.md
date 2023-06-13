# Comparing `tmp/prefect-aws-0.3.2.tar.gz` & `tmp/prefect-aws-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-vsru1pap/prefect-aws-0.3.2.tar", last modified: Thu May 25 19:27:14 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-1ip9v5mt/prefect-aws-0.3.3.tar", last modified: Tue Jun 13 17:03:32 2023, max compression
```

## Comparing `prefect-aws-0.3.2.tar` & `prefect-aws-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    57767 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/ecs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56892 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/prefect_aws/workers/ecs_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/prefect_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:27:14.000000 prefect-aws-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    67274 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26625 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/tests/test_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-05-25 19:25:31.000000 prefect-aws-0.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57782 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/ecs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/projects/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/secrets_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56907 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/workers/ecs_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26625 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/versioneer.py
```

### Comparing `prefect-aws-0.3.2/LICENSE` & `prefect-aws-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/PKG-INFO` & `prefect-aws-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.2
+Version: 0.3.3
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.2 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.3 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.2/README.md` & `prefect-aws-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/batch.py` & `prefect-aws-0.3.3/prefect_aws/batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/client_parameters.py` & `prefect-aws-0.3.3/prefect_aws/client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/client_waiter.py` & `prefect-aws-0.3.3/prefect_aws/client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/credentials.py` & `prefect-aws-0.3.3/prefect_aws/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/ecs.py` & `prefect-aws-0.3.3/prefect_aws/ecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,18 +112,18 @@
 import time
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple, Union
 
 import boto3
 import yaml
 from anyio.abc import TaskStatus
-from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.infrastructure.base import Infrastructure, InfrastructureResult
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
+from prefect.utilities.dockerutils import get_prefect_image_name
 from prefect.utilities.pydantic import JsonPatch
 from pydantic import Field, root_validator, validator
 from slugify import slugify
 from typing_extensions import Literal, Self
 
 from prefect_aws import AwsCredentials
 from prefect_aws.workers.ecs_worker import _TAG_REGEX
```

### Comparing `prefect-aws-0.3.2/prefect_aws/projects/steps.py` & `prefect-aws-0.3.3/prefect_aws/projects/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/s3.py` & `prefect-aws-0.3.3/prefect_aws/s3.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/secrets_manager.py` & `prefect-aws-0.3.3/prefect_aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/prefect_aws/workers/ecs_worker.py` & `prefect-aws-0.3.3/prefect_aws/workers/ecs_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 from typing import Any, Dict, Generator, List, NamedTuple, Optional, Tuple
 from uuid import UUID
 
 import anyio
 import anyio.abc
 import boto3
 import yaml
-from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import FlowRun
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
+from prefect.utilities.dockerutils import get_prefect_image_name
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
 from pydantic import Field, root_validator
```

### Comparing `prefect-aws-0.3.2/prefect_aws.egg-info/PKG-INFO` & `prefect-aws-0.3.3/prefect_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.2
+Version: 0.3.3
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.2 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.3 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.2/prefect_aws.egg-info/SOURCES.txt` & `prefect-aws-0.3.3/prefect_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/setup.cfg` & `prefect-aws-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/setup.py` & `prefect-aws-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/tests/test_batch.py` & `prefect-aws-0.3.3/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/tests/test_block_standards.py` & `prefect-aws-0.3.3/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/tests/test_client_parameters.py` & `prefect-aws-0.3.3/tests/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/tests/test_client_waiter.py` & `prefect-aws-0.3.3/tests/test_client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/tests/test_credentials.py` & `prefect-aws-0.3.3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/tests/test_ecs.py` & `prefect-aws-0.3.3/tests/test_ecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 import anyio
 import pytest
 import yaml
 from botocore.exceptions import ClientError
 from moto import mock_ec2, mock_ecs, mock_logs
 from moto.ec2.utils import generate_instance_identity_document
-from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.logging.configuration import setup_logging
 from prefect.server.schemas.core import Deployment, Flow, FlowRun
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
+from prefect.utilities.dockerutils import get_prefect_image_name
 from pydantic import ValidationError
 
 from prefect_aws.ecs import (
     ECS_DEFAULT_CPU,
     ECS_DEFAULT_MEMORY,
     ECSTask,
     get_container,
```

### Comparing `prefect-aws-0.3.2/tests/test_s3.py` & `prefect-aws-0.3.3/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/tests/test_secrets_manager.py` & `prefect-aws-0.3.3/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.2/versioneer.py` & `prefect-aws-0.3.3/versioneer.py`

 * *Files identical despite different names*

