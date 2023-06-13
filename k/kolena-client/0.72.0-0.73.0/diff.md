# Comparing `tmp/kolena_client-0.72.0.tar.gz` & `tmp/kolena_client-0.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.72.0.tar", max compression
+gzip compressed data, was "kolena_client-0.73.0.tar", max compression
```

## Comparing `kolena_client-0.72.0.tar` & `kolena_client-0.73.0.tar`

### file list

```diff
@@ -1,102 +1,107 @@
--rw-r--r--   0        0        0    11346 2023-06-06 18:23:38.824339 kolena_client-0.72.0/LICENSE
--rw-r--r--   0        0        0      556 2023-06-06 18:23:38.824339 kolena_client-0.72.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1546 2023-06-06 18:23:38.824339 kolena_client-0.72.0/README.md
--rw-r--r--   0        0        0     1356 2023-06-06 18:32:46.536566 kolena_client-0.72.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     8201 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5540 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      783 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4970 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3566 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3255 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4468 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8566 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13755 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12341 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13033 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5327 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20512 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9316 2023-06-06 18:23:38.828340 kolena_client-0.72.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14583 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12193 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16915 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15376 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3544 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/initialize.py
--rw-r--r--   0        0        0     4550 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6281 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     8158 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    18695 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    10725 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3424 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3498 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      846 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0    14420 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7589 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13426 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22768 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     9223 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    14458 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9349 2023-06-06 18:23:38.832340 kolena_client-0.72.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     2560 2023-06-06 18:32:46.536566 kolena_client-0.72.0/pyproject.toml
--rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 kolena_client-0.72.0/setup.py
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 kolena_client-0.72.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-13 21:32:39.845196 kolena_client-0.73.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-06-13 21:32:39.845196 kolena_client-0.73.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     2276 2023-06-13 21:32:39.845196 kolena_client-0.73.0/README.md
+-rw-r--r--   0        0        0     1356 2023-06-13 21:38:32.867401 kolena_client-0.73.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     4153 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5540 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     2520 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      786 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-06-13 21:32:39.877198 kolena_client-0.73.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      783 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4970 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8851 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13920 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13600 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20960 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10130 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14750 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16125 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3865 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/initialize.py
+-rw-r--r--   0        0        0     2474 2023-06-13 21:32:39.881199 kolena_client-0.73.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13877 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    21534 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      964 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0    15527 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8265 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    14301 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22734 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    10564 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15251 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9419 2023-06-13 21:32:39.885199 kolena_client-0.73.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3048 2023-06-13 21:38:32.867401 kolena_client-0.73.0/pyproject.toml
+-rw-r--r--   0        0        0     4658 1970-01-01 00:00:00.000000 kolena_client-0.73.0/PKG-INFO
```

### Comparing `kolena_client-0.72.0/LICENSE` & `kolena_client-0.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/LICENSE_HEADER` & `kolena_client-0.73.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/README.md` & `kolena_client-0.73.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />
+  <img src="/docs/assets/images/wordmark-violet.svg" width="400" alt="Kolena" />
 </p>
 
 <p align='center'>
   <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena" /></a>
   <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena" /></a>
   <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk" /></a>
   <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1"/></a>
@@ -19,12 +19,42 @@
 - Understand and track behavioral improvements and regressions
 - Meaningfully communicate model capabilities
 - Automate model testing and deployment workflows
 
 This `kolena` package contains the Python client library for programmatic interaction with the Kolena ML testing
 platform.
 
+## Setup
+
+Client builds can be installed directly from PyPI using any Python package manager such as pip:
+
+```zsh
+pip install kolena
+```
+
+Advanced use cases (eg. metrics computation) may require extra dependencies which can be installed by running:
+```zsh
+pip install kolena[metrics]
+```
+
+<details>
+<summary>Installing with <a href="https://python-poetry.org/">Poetry</a></summary>
+<br>
+Install project dependencies by running
+
+```zsh
+poetry update && poetry install
+```
+
+Extra dependencies such as [Scikit-learn](https://scikit-learn.org/stable/) can be included by running
+```zsh
+poetry install --all-extras
+```
+</details>
+
+For more information, see the [installation documentation](https://docs.kolena.io/testing-with-kolena/using-kolena-client#installation).
+
 ## Documentation
 
 Visit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the
 [API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena` typing and
 function documentation.
```

#### html2text {}

```diff
@@ -5,12 +5,20 @@
               [https://img.shields.io/badge/resource-docs-6434c1]
 --- [Kolena](https://www.kolena.io) is a comprehensive machine learning testing
 and debugging platform to surface hidden model behaviors and take the mystery
 out of model development. Kolena helps you: - Perform high-resolution model
 evaluation - Understand and track behavioral improvements and regressions -
 Meaningfully communicate model capabilities - Automate model testing and
 deployment workflows This `kolena` package contains the Python client library
-for programmatic interaction with the Kolena ML testing platform. ##
-Documentation Visit [docs.kolena.io](https://docs.kolena.io/) for tutorial and
-usage documentation and the [API Reference](https://app.kolena.io/api/
-developer/docs/html/index.html) for detailed `kolena` typing and function
-documentation.
+for programmatic interaction with the Kolena ML testing platform. ## Setup
+Client builds can be installed directly from PyPI using any Python package
+manager such as pip: ```zsh pip install kolena ``` Advanced use cases (eg.
+metrics computation) may require extra dependencies which can be installed by
+running: ```zsh pip install kolena[metrics] ```  Installing with Poetry
+Install project dependencies by running ```zsh poetry update && poetry install
+``` Extra dependencies such as [Scikit-learn](https://scikit-learn.org/stable/
+) can be included by running ```zsh poetry install --all-extras ```  For more
+information, see the [installation documentation](https://docs.kolena.io/
+testing-with-kolena/using-kolena-client#installation). ## Documentation Visit
+[docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation
+and the [API Reference](https://app.kolena.io/api/developer/docs/html/
+index.html) for detailed `kolena` typing and function documentation.
```

### Comparing `kolena_client-0.72.0/kolena/__init__.py` & `kolena_client-0.73.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/__init__.py` & `kolena_client-0.73.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/__init__.py` & `kolena_client-0.73.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.73.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/client_log.py` & `kolena_client-0.73.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/detection.py` & `kolena_client-0.73.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/fr.py` & `kolena_client-0.73.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/generic.py` & `kolena_client-0.73.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/repository.py` & `kolena_client-0.73.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/token.py` & `kolena_client-0.73.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_api/v1/workflow.py` & `kolena_client-0.73.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/__init__.py` & `kolena_client-0.73.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.73.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/batched_load.py` & `kolena_client-0.73.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/cli.py` & `kolena_client-0.73.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/consts.py` & `kolena_client-0.73.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.73.0/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.73.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/datatypes.py` & `kolena_client-0.73.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/endpoints.py` & `kolena_client-0.73.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/frozen.py` & `kolena_client-0.73.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/geometry.py` & `kolena_client-0.73.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/inference_validators.py` & `kolena_client-0.73.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/instrumentation.py` & `kolena_client-0.73.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/krequests.py` & `kolena_client-0.73.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/log.py` & `kolena_client-0.73.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/repository.py` & `kolena_client-0.73.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/serde.py` & `kolena_client-0.73.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/serializable.py` & `kolena_client-0.73.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/state.py` & `kolena_client-0.73.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.73.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/_utils/validators.py` & `kolena_client-0.73.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/classification/__init__.py` & `kolena_client-0.73.0/kolena/classification/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # noreorder
 from kolena._api.v1.detection import CustomMetrics
 from .test_config import TestConfig
+from .test_config import FixedGlobalThreshold
+from .test_config import AccuracyOptimal
 from .test_image import TestImage
 from .test_case import TestCase
 from .test_suite import TestSuite
 from .model import Model
 from .model import InferenceModel
 from .test_run import CustomMetricsCallback
 from .test_run import TestRun
 from .test_run import test
 
 __all__ = [
     "TestConfig",
+    "FixedGlobalThreshold",
+    "AccuracyOptimal",
     "TestImage",
     "TestCase",
     "TestSuite",
     "Model",
     "InferenceModel",
     "CustomMetrics",
     "CustomMetricsCallback",
```

### Comparing `kolena_client-0.72.0/kolena/classification/metadata.py` & `kolena_client-0.73.0/kolena/classification/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Metadata associated with a :class:`kolena.classification.TestImage`.
+Metadata associated with a [`TestImage`][kolena.classification.TestImage].
 
-.. code-block:: python
+```python
+from kolena.classification import TestImage
+from kolena.classification.metadata import Landmarks, BoundingBox, Asset
 
-    test_image = TestImage("s3://bucket/path/to/image.png", metadata=dict(
-        input_landmarks=Landmarks(*landmarks),
-        input_bounding_box=BoundingBox(*bounding_box),
-        image_grayscale=Asset("s3://bucket/path/to/image_grayscale.png"),
-    ))
+test_image = TestImage("s3://bucket/path/to/image.png", metadata=dict(
+    input_landmarks=Landmarks([(0,0), (10, 10), (20, 20), (30, 30), (40, 40)]),
+    input_bounding_box=BoundingBox((0, 0), (100, 100)),
+    image_grayscale=Asset("s3://bucket/path/to/image_grayscale.png"),
+))
+```
 """
 from kolena.detection._internal.metadata import Annotation
 from kolena.detection._internal.metadata import Asset
 from kolena.detection._internal.metadata import BoundingBox
 from kolena.detection._internal.metadata import Landmarks
 from kolena.detection._internal.metadata import MetadataElement
```

### Comparing `kolena_client-0.72.0/kolena/classification/model.py` & `kolena_client-0.73.0/kolena/classification/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,23 +29,28 @@
 from kolena.detection._datatypes import LoadInferencesDataFrame
 from kolena.detection._internal import BaseModel
 from kolena.detection.inference import ClassificationLabel
 
 
 class Model(BaseModel):
     """
-    The descriptor for a classification model in the Kolena platform.
+    The descriptor for a classification model in Kolena.
+
+    For additional functionality, see the associated
+    [base class documentation][kolena.detection._internal.model.BaseModel].
     """
 
-    #: Unique name of the model, potentially containing information about the architecture, training dataset,
-    #: configuration, framework, commit hash, etc.
     name: str
+    """
+    Unique name of the model, potentially containing information about the architecture, training dataset,
+    configuration, framework, commit hash, etc.
+    """
 
-    #: Unstructured metadata associated with the model.
     metadata: Dict[str, Any]
+    """Unstructured metadata associated with the model."""
 
     _TestImageClass = TestImage
     _TestCaseClass = TestCase
     _TestSuiteClass = TestSuite
     _InferenceClass = Tuple[str, float]
     _LoadInferencesDataFrameClass = LoadInferencesDataFrame
 
@@ -64,21 +69,23 @@
             if isinstance(inference, ClassificationLabel)
         ]
         return test_image, inferences
 
 
 class InferenceModel(Model):
     """
-    A :class:`kolena.classification.Model` with a special :meth:`kolena.classification.InferenceModel.infer` member
-    performing inference on a provided :class:`kolena.classification.TestImage`.
+    A [`Model`][kolena.classification.Model] with a special [`infer`][kolena.classification.InferenceModel.infer] member
+    performing inference on a provided [`TestImage`][kolena.classification.TestImage].
     """
 
-    #: A function transforming an input :class:`kolena.classification.TestImage` to zero or more ``(label, confidence)``
-    #: tuples representing model predictions.
     infer: Callable[[TestImage], Optional[List[Tuple[str, float]]]]
+    """
+    A function transforming an input [`TestImage`][kolena.classification.TestImage] to zero or more
+    `(label, confidence)` tuples representing model predictions.
+    """
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
         self,
         name: str,
         infer: Callable[[TestImage], Optional[List[Tuple[str, float]]]],
         metadata: Optional[Dict[str, Any]] = None,
```

### Comparing `kolena_client-0.72.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.73.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.73.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.73.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.73.0/kolena/classification/multiclass/test_run.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 from kolena.workflow import EvaluatorConfiguration
 from kolena.workflow.test_run import test as base_test
 from kolena.workflow.test_run import TestRun as BaseTestRun
 
 
 class TestRun(BaseTestRun):
     """
-    Convenience alias for :class:`kolena.workflow.test_run.TestRun`, configured for the
+    Convenience alias for [`kolena.workflow.TestRun`][kolena.workflow.test_run.TestRun], configured for the
     `kolena.classification.multiclass` workflow and evaluator.
 
-    Interface to run tests for a :class:`kolena.classification.multiclass.Model` on a set of
-    :class:`kolena.classification.multiclass.TestSuite` suites.
+    Interface to run tests for a [`Model`][kolena.classification.multiclass.Model] on a
+    [`TestSuite`][kolena.classification.multiclass.TestSuite].
 
-    For a streamlined interface, see :meth:`kolena.classification.multiclass.test`.
+    For a streamlined interface, see [`test`][kolena.classification.multiclass.test].
 
-    :param model: the model being tested.
-    :param test_suite: the test suite on which to test the model.
-    :param reset: overwrites existing inferences if set.
+    :param model: The model being tested.
+    :param test_suite: The test suite on which to test the model.
+    :param reset: Overwrites existing inferences if set.
     """
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
         self,
         model: Model,
         test_suite: TestSuite,
@@ -64,26 +64,26 @@
 def test(
     model: Model,
     test_suite: TestSuite,
     configurations: Optional[List[EvaluatorConfiguration]] = None,
     reset: bool = False,
 ) -> None:
     """
-    Convenience alias for :meth:`kolena.workflow.test_run.test` configured for the `kolena.classification.multiclass`
-    workflow and evaluator.
+    Convenience alias for [`test`][kolena.workflow.test] configured for the `kolena.classification.multiclass` workflow
+    and evaluator.
 
-    Tests the provided :class:`kolena.classification.multiclass.Model`` on the provided
-    :class:`kolena.classification.multiclass.TestSuite` suite. Any tests already in progress for this model on this
+    Tests the provided [`Model`][kolena.classification.multiclass.Model] on the provided
+    [`TestSuite`][kolena.classification.multiclass.TestSuite]. Any test already in progress for this model on this
     test suite is resumed.
 
-    :param model: the model being tested, implementing the ``infer`` method.
-    :param test_suite: the test suite on which to test the model.
-    :param configurations: an optional list of configurations to use when running the evaluator. Defaults to selecting
+    :param model: The model being tested, implementing the `infer` method.
+    :param test_suite: The test suite on which to test the model.
+    :param configurations: An optional list of configurations to use when running the evaluator. Defaults to selecting
         the max confidence label (with no thresholding) if unset.
-    :param reset: overwrites existing inferences if set.
+    :param reset: Overwrites existing inferences if set.
     """
     if configurations is None:
         configurations = [ThresholdConfiguration()]
     base_test(
         model=model,
         test_suite=test_suite,
         evaluator=MulticlassClassificationEvaluator,
```

### Comparing `kolena_client-0.72.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.73.0/kolena/classification/multiclass/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,24 +38,20 @@
 
 
 @dataclass(frozen=True)
 class GroundTruth(BaseGroundTruth):
     classification: ClassificationLabel
 
 
+# DEPRECATED: preserved for compatibility only. Please use ScoredClassificationLabel instead
 @dataclass(frozen=True)
 class InferenceLabel(ClassificationLabel):
-    """
-    :class:`InferenceLabel` is deprecated and preserved for compatibility only. Please use
-    :class:`ScoredClassificationLabel` instead.
-    """
-
     confidence: float
 
-    @deprecated(details="use :class:`kolena.workflow.annotation.ScoredClassificationLabel`", deprecated_in="0.70.0")
+    @deprecated(details="use `kolena.workflow.annotation.ScoredClassificationLabel`", deprecated_in="0.70.0")
     def __post_init__(self) -> None:
         ...
 
     @property
     def score(self) -> float:
         return self.confidence
```

### Comparing `kolena_client-0.72.0/kolena/classification/test_case.py` & `kolena_client-0.73.0/kolena/classification/test_case.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,24 @@
 
     Fundamentally, a test case can be thought of as a benchmark dataset. Metrics are computed for each test case.
 
     A test case may be as large or as small as necessary. A test case may have millions of images for high-level results
     across a large population. Alternatively, a test case may have only one or a handful of images for laser-focus on a
     specific scenario.
 
-    :param name: the name of the test case. If a test case by this name already exists, that test case is loaded
-    :param version: optionally specify the version of the test case to load. Ignored when a test case by the
-        provided name does not already exist
-    :param description: optionally specify a description for the new test case. Ignored when a test case with the
-        provided name already exists
-    :param images: optionally provide a list of :class:`kolena.classification.TestImage` images used to seed a new test
-        case. Ignored when a test case with the provided name already exists
+    For additional functionality, see the associated
+    [base class documentation][kolena.detection._internal.test_case.BaseTestCase].
+
+    :param name: The name of the test case. If a test case by this name already exists, that test case is loaded.
+    :param version: Optionally specify the version of the test case to load. Ignored when a test case by the
+        provided name does not already exist.
+    :param description: Optionally specify a description for the new test case. Ignored when a test case with the
+        provided name already exists.
+    :param images: Optionally provide a list of [`TestImage`][kolena.classification.TestImage] images used to seed a new
+        test case. Ignored when a test case with the provided name already exists.
     """
 
     _TestImageClass = TestImage
     _TestImageDataFrameClass = TestImageDataFrame
 
     _workflow = WorkflowType.CLASSIFICATION
```

### Comparing `kolena_client-0.72.0/kolena/classification/test_config.py` & `kolena_client-0.73.0/kolena/classification/test_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 # limitations under the License.
 from kolena._api.v1.detection import Metrics
 from kolena.detection._internal import TestConfig as _TestConfig
 from kolena.errors import InputValidationError
 
 
 class TestConfig(_TestConfig):
-    ...
+    """
+    Base class for testing configurations.
+
+    See concrete implementations [`FixedGlobalThreshold`][kolena.classification.FixedGlobalThreshold] and
+    [`AccuracyOptimal`][kolena.classification.AccuracyOptimal] for details.
+    """
 
 
 class FixedGlobalThreshold(TestConfig):
     """
-    Test configuration that sets the default display threshold in the Kolena UI to be a fixed global threshold for all
-    label classes within the test run.
+    Test configuration that sets the default display threshold in Kolena to a fixed global threshold for all labels
+    within the test suite.
     """
 
-    # The threshold used as the default when visualizing results in the Kolena UI.
-    # Must be between 0 and 1.
     fixed_threshold: float
+    """The threshold used as the default when visualizing results in Kolena. Must be between 0 and 1."""
 
     def __init__(self, fixed_threshold: float):
         if fixed_threshold < 0 or fixed_threshold > 1:
             raise InputValidationError(f"threshold of {fixed_threshold} was not between 0 and 1")
         self.fixed_threshold = fixed_threshold
 
     def _to_run_config(self) -> Metrics.RunConfig:
@@ -41,18 +45,18 @@
             iou_threshold=0,
             params=dict(threshold=self.fixed_threshold),
         )
 
 
 class AccuracyOptimal(TestConfig):
     """
-    Test configuration that sets the default display threshold in the Kolena UI to be dynamically set to the threshold
-    that corresponds to the highest accuracy score for the test suite within the test run.
+    Test configuration that sets the default display threshold in Kolena to the threshold that corresponds to the
+    highest accuracy score across all images within the test suite being tested.
 
-    This threshold is evaluated and set per label for test suites with multiple label classes.
+    This threshold is evaluated and set per label for test suites with multiple labels.
     """
 
     def __init__(self) -> None:
         ...
 
     def _to_run_config(self) -> Metrics.RunConfig:
         return Metrics.RunConfig(strategy=Metrics.RunStrategy.ACCURACY_OPTIMAL, iou_threshold=0)
```

### Comparing `kolena_client-0.72.0/kolena/classification/test_image.py` & `kolena_client-0.73.0/kolena/classification/test_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,39 +26,41 @@
 from kolena.detection._internal.metadata import MetadataElement
 from kolena.detection._internal.test_image import BaseTestImage
 from kolena.detection.ground_truth import ClassificationLabel
 from kolena.detection.ground_truth import GroundTruth
 
 
 class TestImage(BaseTestImage):
-    """
-    An image with associated ground truth labels for testing.
-    """
+    """An image with associated ground truth labels for testing."""
 
-    #: Pointer to the bucket location of this image, e.g. ``gs://my-bucket/my-dataset/example.png``.
     locator: str
+    """Pointer to the bucket location of this image, e.g. `gs://my-bucket/my-dataset/example.png`."""
 
-    #: The source dataset this image belongs to.
     dataset: str
+    """The source dataset this image belongs to."""
 
-    #: Zero or more ground truth labels for this image. For binary classifiers, an arbitrary string such as ``positive``
-    #: may be used. Not surfaced during testing.
     labels: List[str]
+    """
+    Zero or more ground truth labels for this image. For binary classifiers, an arbitrary string such as `positive`
+    may be used. Not surfaced during testing.
+    """
 
-    #: Arbitrary metadata associated with this image. This metadata is surfaced during testing and may be used as model
-    #: inputs as necessary.
-    #:
-    #: Certain metadata values can be visualized in the web platform when viewing results:
-    #:
-    #: * :class:`kolena.classification.metadata.Annotation` objects are overlaid on the main image
-    #: * :class:`kolena.classification.metadata.Asset` objects containing locators pointing to images, e.g.
-    #:   ``gs://my-bucket/my-dataset/example-1channel.png``, are displayed
-    #:
-    #: See :mod:`kolena.classification.metadata` documentation for more details.
     metadata: Dict[str, MetadataElement]
+    """
+    Arbitrary metadata associated with this image. This metadata is surfaced during testing and may be used as model
+    inputs as necessary.
+
+    Certain metadata values can be visualized in the web platform when viewing results:
+
+    - [`Annotation`][kolena.classification.metadata.Annotation] objects are overlaid on the main image
+    - [`Asset`][kolena.classification.metadata.Asset] objects containing locators pointing to images, e.g.
+        ``gs://my-bucket/my-dataset/example-1channel.png``, are displayed
+
+    See the [metadata documentation][kolena.classification.metadata.Annotation] for more details.
+    """
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
         self,
         locator: str,
         dataset: Optional[str] = None,
         labels: Optional[List[str]] = None,
@@ -68,17 +70,17 @@
         self.labels = labels or []
 
     def filter(self, predicate: Callable[[str], bool]) -> "TestImage":
         """
         Return a copy of this test image with ground truth labels filtered to only those that match the provided
         predicate.
 
-        :param predicate: function accepting a string label and returning a boolean indicating whether or not to include
-            the ground truth label
-        :return: a new test image with labels filtered by the predicate
+        :param predicate: Function accepting a string label and returning a boolean indicating whether or not to include
+            the ground truth label.
+        :return: A new test image with labels filtered by the predicate.
         """
         return TestImage(**{**self._fields(), "labels": [label for label in self.labels if predicate(label)]})
 
     @classmethod
     def _meta_keys(cls) -> List[str]:
         return detection.TestImage._meta_keys()
```

### Comparing `kolena_client-0.72.0/kolena/classification/test_run.py` & `kolena_client-0.73.0/kolena/classification/test_run.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,28 +33,29 @@
 from kolena.detection._internal.metadata import _from_dict
 from kolena.detection._internal.test_run import CustomMetricsCallback
 from kolena.detection.inference import ClassificationLabel
 
 
 class TestRun(BaseTestRun):
     """
-    Interface to run tests for a :class:`kolena.classification.Model` on a set of
-    :class:`kolena.classification.TestSuite` suites. Any in-progress tests for this model on these suites are resumed.
+    Interface to run tests for a [`Model`][kolena.classification.Model] on a
+    [`TestSuite`][kolena.classification.TestSuite]. Any in-progress tests for this model on these suites are resumed.
 
-    For a streamlined interface, see :meth:`kolena.classification.test`.
+    For a streamlined interface, see [`test`][kolena.classification.test].
 
-    :param model: the model being tested.
-    :param test_suite: the test suite on which to test the model.
-    :param test_config: Optionally specify a :class:`kolena.classification.TestConfig` to customize the metrics
-                           evaluation logic for this test run.
-                           Defaults to :class:`kolena.classification.test_config.AccuracyOptimal` if unspecified.
+    :param model: The model being tested.
+    :param test_suite: The test suite on which to test the model.
+    :param test_config: Optionally specify a configuration, e.g.
+        [`FixedGlobalThreshold`][kolena.classification.FixedGlobalThreshold], to customize the metrics evaluation logic
+        for this test run. Defaults to [`AccuracyOptimal`][kolena.classification.test_config.AccuracyOptimal] if
+        unspecified.
     :param custom_metrics_callback: Optionally specify a callback function to compute custom metrics for each test-case.
-                                        The callback would be passed inferences of images in each testcase and should
-                                        return a dictionary with metric name as key and metric value as value.
-    :param reset: overwrites existing inferences if set.
+        The callback would be passed inferences of images in each testcase and should return a dictionary with metric
+        name as key and metric value as value.
+    :param reset: Overwrites existing inferences if set.
     """
 
     _TestImageClass = TestImage
     _InferenceClass = Tuple[str, float]
     _ImageResultDataFrameClass: Type[ImageResultDataFrame] = ImageResultDataFrame
     _LoadTestImagesDataFrameClass: Type[LoadTestImagesDataFrame] = LoadTestImagesDataFrame
 
@@ -100,28 +101,29 @@
     model: InferenceModel,
     test_suite: TestSuite,
     test_config: Optional[TestConfig] = None,
     custom_metrics_callback: Optional[CustomMetricsCallback[TestImage, Tuple[str, float]]] = None,
     reset: bool = False,
 ) -> None:
     """
-    Test the provided :class:`kolena.classification.InferenceModel`` on one or more provided
-    :class:`kolena.detection.TestSuite` suites. Any tests already in progress for this model on these suites are
+    Test the provided [`InferenceModel`][kolena.classification.InferenceModel] on a
+    [`TestSuite`][kolena.classification.TestSuite]. Any tests already in progress for this model on these suites are
     resumed.
 
-    :param model: the model being tested, complete with :meth:`kolena.classification.InferenceModel.infer` function
-        to perform inference.
-    :param test_suite: the test suite on which to test the model.
-    :param test_config: Optionally specify a :class:`kolena.classification.TestConfig` to customize the metrics
-                           evaluation logic for this test run.
-                           Defaults to :class:`kolena.classification.test_config.AccuracyOptimal` if unspecified.
-    :param custom_metrics_callback: Optionally specify a callback function to compute custom metrics for each test-case.
-                                        The callback would be passed inferences of images in each testcase and should
-                                        return a dictionary with metric name as key and metric value as value.
-    :param reset: overwrites existing inferences if set.
+    :param model: The model being tested, complete with an
+        [`InferenceModel.infer`][kolena.classification.InferenceModel.infer] function to perform inference.
+    :param test_suite: The test suite on which to test the model.
+    :param test_config: Optionally specify a configuration, e.g.
+        [`FixedGlobalThreshold`][kolena.classification.FixedGlobalThreshold], to customize the metrics evaluation logic
+        for this test run. Defaults to [`AccuracyOptimal`][kolena.classification.test_config.AccuracyOptimal] if
+        unspecified.
+    :param custom_metrics_callback: Optionally specify a callback function to compute custom metrics for each test case.
+        The callback would be passed inferences of images in each testcase and should return a dictionary with metric
+        name as key and metric value as value.
+    :param reset: Overwrites existing inferences if set.
     """
     with TestRun(
         model,
         test_suite,
         test_config=test_config,
         custom_metrics_callback=custom_metrics_callback,
         reset=reset,
```

### Comparing `kolena_client-0.72.0/kolena/classification/test_suite.py` & `kolena_client-0.73.0/kolena/classification/test_suite.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,41 +18,51 @@
 from kolena._api.v1.workflow import WorkflowType
 from kolena.classification import TestCase
 from kolena.detection._internal import BaseTestSuite
 
 
 class TestSuite(BaseTestSuite):
     """
-    A test suite is a grouping of :class:`kolena.classification.TestCase` tests.
+    A test suite is a grouping of [`TestCase`][kolena.classification.TestCase] objects.
 
-    Testing on test suites is performed via :mod:`kolena.classification.test`. Metrics are computed across all samples
-    in a test suite and also for each individual test case within the suite.
+    Testing on test suites is performed via [`test`][kolena.classification.test]. Metrics are computed across all
+    samples in a test suite and also for each individual test case within the suite.
 
-    :param name: the name of the test suite. If a test suite by this name already exists, that test suite is loaded
-    :param version: optionally specify the version of the test suite to load. Ignored when the a suite by the
-        provided name does not already exist
-    :param description: optionally specify a description for the new test suite. Ignored when a test suite with the
-        provided name already exists
-    :param test_cases: optionally provide a list of :class:`kolena.classification.TestCase` tests used to seed a new
-        test suite. Ignored when a test suite with the provided name already exists
+    For additional functionality, see the associated
+    [base class documentation][kolena.detection._internal.test_suite.BaseTestSuite].
+
+    :param name: The name of the test suite. If a test suite by this name already exists, that test suite is loaded.
+    :param version: Optionally specify the version of the test suite to load. Ignored when the a suite by the
+        provided name does not already exist.
+    :param description: Optionally specify a description for the new test suite. Ignored when a test suite with the
+        provided name already exists.
+    :param test_cases: Optionally provide a list of [`TestCase`][kolena.classification.TestCase] tests used to seed a
+        new test suite. Ignored when a test suite with the provided name already exists.
     """
 
-    #: Unique name of the test suite.
     name: str
+    """Unique name of the test suite."""
 
-    #: The version of the test suite. Version is automatically incremented whenever the test suite is modified via
-    #: :meth:`TestSuite.edit`.
     version: int
+    """
+    The version of the test suite. Version is automatically incremented whenever the test suite is modified via
+    [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
+    """
 
-    #: Free-form description of this test suite. May be edited at any time via :meth:`TestSuite.edit`.
     description: str
+    """
+    Free-form description of this test suite. May be edited at any time via
+    [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
+    """
 
-    #: The :class:`kolena.classification.TestCase` tests in this test suite. May be edited at any time via
-    #: :meth:`TestSuite.edit`.
     test_cases: List[TestCase]
+    """
+    The [`TestCase`][kolena.classification.TestCase] objects in this test suite. May be edited at any time via
+    [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
+    """
 
     _id: int
     _workflow: WorkflowType = WorkflowType.CLASSIFICATION
 
     def __init__(
         self,
         name: str,
```

### Comparing `kolena_client-0.72.0/kolena/detection/__init__.py` & `kolena_client-0.73.0/kolena/detection/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # limitations under the License.
 
 # noreorder
 from kolena._api.v1.detection import CustomMetrics
 from .ground_truth import GroundTruth
 from .inference import Inference
 from .test_config import TestConfig
+from .test_config import FixedGlobalThreshold
+from .test_config import F1Optimal
 from .test_image import TestImage
 from .test_image import iter_images
 from .test_image import load_images
 from .test_case import TestCase
 from .test_suite import TestSuite
 from .model import Model
 from .model import InferenceModel
@@ -28,14 +30,16 @@
 from .test_run import TestRun
 from .test_run import test
 
 __all__ = [
     "GroundTruth",
     "Inference",
     "TestConfig",
+    "FixedGlobalThreshold",
+    "F1Optimal",
     "TestImage",
     "iter_images",
     "load_images",
     "TestCase",
     "TestSuite",
     "InferenceModel",
     "Model",
```

### Comparing `kolena_client-0.72.0/kolena/detection/_datatypes.py` & `kolena_client-0.73.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.73.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.73.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.73.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/inference.py` & `kolena_client-0.73.0/kolena/detection/_internal/inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,17 +22,10 @@
 class InferenceType(str, Enum):
     CLASSIFICATION_LABEL = "CLASSIFICATION_LABEL"
     BOUNDING_BOX = "BOUNDING_BOX"
     SEGMENTATION_MASK = "SEGMENTATION_MASK"
 
 
 class Inference(Serializable, Frozen, metaclass=ABCMeta):
-    """
-    Base class for an inference associated with an image.
-
-    See concrete implementations :class:`kolena.detection.inference.ClassificationLabel`,
-    :class:`kolena.detection.inference.BoundingBox`, :class:`kolena.detection.inference.SegmentationMask`, for details.
-    """
-
     @abstractmethod
     def __init__(self) -> None:
         ...
```

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.73.0/kolena/detection/_internal/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     """
     An asset living in your shared bucket. Assets are surfaced during testing along with any other metadata associated
     with a given test image.
 
     In the web platform, certain assets such as PNG and JPG images are viewable when visualizing results in the gallery.
     """
 
-    #: Location of this asset in shared bucket, e.g. ``s3://my-bucket/path/to/image.png``.
     locator: str
+    """Location of this asset in shared bucket, e.g. `s3://my-bucket/path/to/image.png`."""
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, locator: str):
         self.locator = locator  # TODO: validate locator
 
     def _to_dict(self) -> Dict[str, Any]:
         return dict(data_type=MetadataElementType.ASSET.value, data_object=dict(locator=self.locator))
@@ -84,19 +84,19 @@
 
     return {key: dump_element(value) for key, value in metadata.items()}
 
 
 class BoundingBox(Annotation):
     """An annotation comprising a bounding box around an object in an image."""
 
-    #: Point in (x, y) pixel coordinates representing the top left corner of the bounding box.
     top_left: Tuple[float, float]
+    """Point in `(x, y)` pixel coordinates representing the top left corner of the bounding box."""
 
-    #: Point in (x, y) pixel coordinates representing the bottom right corner of the bounding box.
     bottom_right: Tuple[float, float]
+    """Point in `(x, y)` pixel coordinates representing the bottom right corner of the bounding box."""
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, top_left: Tuple[float, float], bottom_right: Tuple[float, float]):
         self.top_left = top_left
         self.bottom_right = bottom_right
 
     def _to_dict(self) -> Dict[str, Any]:
@@ -108,16 +108,16 @@
 
 class Landmarks(Annotation):
     """
     An annotation comprising an arbitrary-length set of landmarks corresponding to some object in an image, e.g. face
     landmarks used for pose estimation.
     """
 
-    #: Any number of (x, y) points in pixel coordinates representing a set of landmarks.
     points: List[Tuple[float, float]]
+    """Any number of `(x, y)` points in pixel coordinates representing a set of landmarks."""
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, points: List[Tuple[float, float]]):
         if len(points) == 0:
             raise ValueError("At least one point required for landmarks annotation.")
         self.points = points
```

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/model.py` & `kolena_client-0.73.0/kolena/detection/_internal/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,23 +51,26 @@
 
 InferenceType = TypeVar("InferenceType")
 SampleInferences = Tuple[TestImageType, Optional[List[InferenceType]]]
 
 
 class BaseModel(ABC, Frozen, WithTelemetry):
     """
-    The descriptor for your model within the Kolena platform.
+    The base class for [`kolena.classification.Model`][kolena.classification.Model] and
+    [`kolena.detection.Model`][kolena.detection.Model].
     """
 
-    #: Unique name of the model within the platform. If the provided model name has already been registered, that model
-    #: and its metadata are loaded upon instantiation.
     name: str
+    """
+    Unique name of the model, potentially containing information about the architecture, training dataset,
+    configuration, framework, commit hash, etc.
+    """
 
-    #: Unstructured metadata associated with the model.
     metadata: Dict[str, Any]
+    """Unstructured metadata associated with the model."""
 
     _id: int
     _workflow: WorkflowType
 
     _TestImageClass: Type[BaseTestImage] = BaseTestImage
     _TestCaseClass: Type[BaseTestCase] = BaseTestCase
     _TestSuiteClass: Type[BaseTestSuite] = BaseTestSuite
@@ -112,24 +115,28 @@
     @validate_arguments(config=ValidatorConfig)
     def load_inferences(
         self,
         test_object: Union[_TestCaseClass, _TestSuiteClass],
     ) -> List[Tuple[_TestImageClass, Optional[List[_InferenceClass]]]]:
         """
         Retrieve the uploaded inferences with identical ground truth labels for each image in a test case or test suite.
+
+        :return: List of all images and inferences from this model on the provided `test_object`.
         """
         return list(self.iter_inferences(test_object))
 
     @validate_arguments(config=ValidatorConfig)
     def iter_inferences(
         self,
         test_object: Union[_TestCaseClass, _TestSuiteClass],
     ) -> Iterator[Tuple[_TestImageClass, Optional[List[_InferenceClass]]]]:
         """
         Iterate the uploaded inferences with identical ground truth labels for each image in a test case or test suite.
+
+        :return: Iterator over all images and inferences from this model on the provided `test_object`.
         """
         for df_batch in self._iter_inference_batch_for_reference(test_object):
             yield from (self._inferences_from_record(record) for record in df_batch.itertuples())
 
     @validate_arguments(config=ValidatorConfig)
     def _iter_inference_batch_for_reference(
         self,
```

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.73.0/kolena/detection/_internal/test_case.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,35 +45,39 @@
 from kolena.workflow._validators import assert_workflows_match
 
 
 class BaseTestCase(ABC, Frozen, WithTelemetry):
     """
     A test case holds a set of images to compute performance metrics against.
 
-    :param name: name of the test case to create or load
-    :param version: optionally specify the version of the test case to load. When absent, the latest version is loaded.
-        Ignored when creating new test cases
-    :param description: optionally specify a description for a newly created test case. For existing test cases, this
-        description can be edited via :meth:`kolena.detection.TestCase.edit`
-    :param images: optionally provide a list of images and associated ground truths to populate a new test case. For
-        existing test cases, images can be edited via :meth:`TestCase.edit`.
+    :param name: Name of the test case to create or load.
+    :param version: Optionally specify the version of the test case to load. When absent, the latest version is loaded.
+        Ignored when creating new test cases.
+    :param description: Optionally specify a description for a newly created test case. For existing test cases, this
+        description can be edited via [`TestCase.edit`][kolena.detection._internal.BaseTestCase.edit].
+    :param images: Optionally provide a list of images and associated ground truths to populate a new test case. For
+        existing test cases, images can be edited via [`TestCase.edit`][kolena.detection._internal.BaseTestCase.edit].
     """
 
     _TestImageClass: Type[BaseTestImage] = BaseTestImage
     _TestImageDataFrameClass: Type[DFType] = DFType
 
-    #: The unique name of this test case. Cannot be changed after creation.
     name: str
+    """The unique name of this test case."""
 
-    #: The version of this test case. A test case's version is automatically incremented whenever it is edited via
-    #: :meth:`TestCase.edit`.
     version: int
+    """
+    The version of this test case. A test case's version is automatically incremented whenever it is edited via
+    [`TestCase.edit`][kolena.detection._internal.BaseTestCase.edit].
+    """
 
-    #: Free-form, human-readable description of this test case. Can be edited at any time via :meth:`TestCase.edit`.
     description: str
+    """Free-form, human-readable description of this test case. Can be edited at any time via
+    [`TestCase.edit`][kolena.detection._internal.BaseTestCase.edit].
+    """
 
     _id: int
     _workflow: WorkflowType
 
     def __init__(
         self,
         name: str,
@@ -188,36 +192,37 @@
         name: str,
         description: Optional[str] = None,
         images: Optional[List[_TestImageClass]] = None,
     ) -> "BaseTestCase":
         """
         Create a new test case with the provided name.
 
-        :param name: the name of the new test case to create.
-        :param description: optional free-form description of the test case to create.
-        :param images: optionally specify a set of images to populate the test case.
-        :return: the newly created test case.
+        :param name: The name of the new test case to create.
+        :param description: Optional free-form description of the test case to create.
+        :param images: Optionally specify a set of images to populate the test case.
+        :return: The newly created test case.
         """
         return cls._create(cls._workflow, name, description, images)
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "BaseTestCase":
         """
         Load an existing test case with the provided name.
-        :param name: the name of the test case to load.
-        :param version: optionally specify a particular version of the test case to load. Defaults to the latest version
+
+        :param name: The name of the test case to load.
+        :param version: Optionally specify a particular version of the test case to load. Defaults to the latest version
             when unset.
-        :return: the loaded test case.
+        :return: The loaded test case.
         """
         data = cls._load_by_name(name, version)
         return cls._create_from_data(data)
 
     class Editor:
         """
-        Interface to edit a test case. Create with :meth:`TestCase.edit`.
+        Interface to edit a test case. Create with [`TestCase.edit`][kolena.detection._internal.BaseTestCase.edit].
         """
 
         _TestImageClass: Type[BaseTestImage] = BaseTestImage
         _images: Dict[str, BaseTestImage]
         _reset: bool
         _description: str
         _initial_description: str
@@ -230,45 +235,45 @@
             self._images: Dict[str, BaseTestImage] = OrderedDict()
 
         @validate_arguments(config=ValidatorConfig)
         def description(self, description: str) -> None:
             """
             Update the description of this test case.
 
-            :param description: the new test case description
+            :param description: The new test case description.
             """
             if self._description == description:
                 return
             self._description = description
             self._edited = True
 
         @validate_arguments(config=ValidatorConfig)
         def add(self, image: _TestImageClass) -> None:
             """
-            Add a test image to the test case, targeting the ``ground_truths`` held by the image.
-            When the test image already exists in the test case, its ground truth
-            is overwritten.
+            Add a test image to the test case, targeting the `ground_truths` held by the image. When the test image
+            already exists in the test case, its ground truth is overwritten.
 
-            To filter the ground truths associated with a test image, see :meth:`kolena.detection.TestImage.filter`.
+            To filter the ground truths associated with a test image, see
+            [`TestImage.filter`][kolena.detection.TestImage.filter].
 
-            :param image: the test image to add to the test case, holding corresponding ground truths
+            :param image: The test image to add to the test case, holding corresponding ground truths.
             """
             if image == self._images.get(image.locator, None):
                 log.info(f"no op: {image.locator} already in test case")
                 return
             self._images[image.locator] = image
             self._edited = True
 
         @validate_arguments(config=ValidatorConfig)
         def remove(self, image: _TestImageClass) -> None:
             """
             Remove the image from the test case.
 
-            :param image: the test image to remove
-            :raises KeyError: if the image is not in the test case
+            :param image: The image to remove.
+            :raises KeyError: The image is not in the test case.
             """
             if image.locator not in self._images.keys():
                 raise KeyError(f"unrecognized image: '{image.locator}' not in test case")
             self._images.pop(image.locator)
             self._edited = True
 
     @classmethod
@@ -281,24 +286,24 @@
         )
 
     @contextmanager
     def edit(self, reset: bool = False) -> Iterator[Editor]:
         """
         Edit this test case in a context:
 
-        .. code-block:: python
-
-            with test_case.edit() as editor:
-                # perform as many editing actions as desired
-                editor.add(...)
-                editor.remove(...)
+        ```python
+        with test_case.edit() as editor:
+            # perform as many editing actions as desired
+            editor.add(...)
+            editor.remove(...)
+        ```
 
-        Changes are committed to the Kolena platform when the context is exited.
+        Changes are committed to Kolena when the context is exited.
 
-        :param reset: clear any and all test samples currently in the test case.
+        :param reset: Clear any and all test samples currently in the test case.
         """
         editor = self.Editor(self.description, reset)
         editor._TestImageClass = self._TestImageClass
         if not reset:
             for image in self.iter_images():
                 editor.add(image)
             editor._edited = False
```

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.73.0/kolena/detection/_internal/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,21 +18,14 @@
 
 from kolena._api.v1.detection import Metrics
 from kolena._utils.frozen import Frozen
 from kolena._utils.serializable import Serializable
 
 
 class TestConfig(Frozen, Serializable, metaclass=ABCMeta):
-    """
-    Base class for a testing configuration.
-
-    See concrete implementations :class:`kolena.detection.config.FixedThreshold`,
-    :class:`kolena.detection.config.F1Optimal` for details.
-    """
-
     @abstractmethod
     def __init__(self) -> None:
         ...
 
     @abstractmethod
     def _to_run_config(self) -> Metrics.RunConfig:
         ...
```

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.73.0/kolena/detection/_internal/test_image.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,23 +27,16 @@
 from kolena.detection._internal.metadata import MetadataElement
 
 
 TestImageType = TypeVar("TestImageType")
 
 
 class BaseTestImage(ABC, Frozen):
-    """Base class for all TestImage classes"""
-
-    #: Bucket locator for the provided test sample, e.g. ``gs://my-bucket/path/to/image.png``.
     locator: str
-
-    #: Dataset this test image belongs to. Empty when unspecified.
     dataset: str
-
-    #: Metadata associated with this test image. Surfaced during test runs.
     metadata: Dict[str, MetadataElement]
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
         self,
         locator: str,
         dataset: Optional[str] = None,
```

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.73.0/kolena/detection/_internal/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 from kolena.errors import CustomMetricsException
 from kolena.errors import IncorrectUsageError
 from kolena.errors import InputValidationError
 from kolena.errors import WorkflowMismatchError
 
 _ImageDataFrame = Union[pa.typing.DataFrame, LoadableDataFrame]
 InferenceType = TypeVar("InferenceType")
+
 CustomMetricsCallback = Callable[[List[SampleInferences]], CustomMetrics]
+"""Signature for a custom metrics computation function."""
 
 
 class BaseTestRun(ABC, Frozen, WithTelemetry):
     """
-    Base interface to run tests
-
-    :param model: the model being tested.
-    :param test_suite: the test suite on which to test the model.
+    The base class for [`kolena.classification.TestRun`][kolena.classification.TestRun] and
+    [`kolena.detection.TestRun`][kolena.detection.TestRun].
     """
 
     _TestImageClass: Type[BaseTestImage] = BaseTestImage
     _InferenceClass: Type[InferenceType] = InferenceType
     _ImageResultDataFrameClass: Type[_ImageDataFrame] = _ImageDataFrame
     _LoadTestImagesDataFrameClass: Type[DFType] = DFType
 
@@ -133,18 +133,18 @@
         self._active = False
         if exc_type is not None:
             report_crash(self._id, API.Path.MARK_CRASHED.value)
 
     @validate_arguments(config=ValidatorConfig)
     def add_inferences(self, image: _TestImageClass, inferences: Optional[List[_InferenceClass]]) -> None:
         """
-        Adds inferences for a test image to the test run results.
+        Add inferences for a test image to the test run results.
 
-        :param image: the image that inferences are evaluated on
-        :param inferences: list of inferences corresponding to the image
+        :param image: The image that inferences are evaluated on.
+        :param inferences: List of inferences corresponding to the image.
         """
         self._assert_active()
 
         if image.locator not in self._locator_to_image_id.keys():
             raise InputValidationError(
                 f"Unrecognized locator '{image.locator}'. Images must be loaded and processed in the same context",
             )
@@ -165,30 +165,27 @@
             self._inferences[image_id] = context_image_inferences
 
         if self._n_inferences >= BatchSize.UPLOAD_RESULTS.value:
             self._upload_chunk()
 
     @validate_arguments(config=ValidatorConfig)
     def iter_images(self) -> Iterator[_TestImageClass]:
-        """
-        Returns an iterator of all remaining images that need inferences evaluated.
-        """
+        """Returns an iterator of all remaining images that need inferences evaluated."""
         self._assert_active()
         for df_image_batch in self._iter_image_batch():
             for record in df_image_batch.itertuples():
                 yield self._image_from_load_image_record(record)
 
     @validate_arguments(config=ValidatorConfig)
     def load_images(self, batch_size: int = BatchSize.LOAD_SAMPLES.value) -> List[_TestImageClass]:
         """
-        Returns a list of images that still need inferences evaluated, bounded in count
-        by batch_size. Note that image ground truths will be excluded from the returned
-        batch of images.
+        Returns a list of images that still need inferences evaluated, bounded in count by `batch_size`. Note that image
+        ground truths will be excluded from the returned batch of images.
 
-        :param batch_size: the maximum number of images to retrieve
+        :param batch_size: The maximum number of images to retrieve.
         """
         self._assert_active()
         log.info("loading batch of images for test run")
         try:
             df_image_batch = next(self._iter_image_batch(batch_size=batch_size))
         except StopIteration:
             # no more images
@@ -229,17 +226,17 @@
             self._id,
             self._model._id,
             self._inferences,
             self._ignored_image_ids,
         )
         df_chunk_serializable = df_chunk.as_serializable()
         upload_data_frame_chunk(df_chunk_serializable, load_uuid=self._upload_uuid)
+        log.success(f"uploaded {self._n_inferences} inferences for test run")
         self._n_inferences = 0
         self._inferences = OrderedDict()
-        log.success(f"uploaded {self._n_inferences} inferences for test run")
 
     def _finalize_upload(self) -> None:
         if self._upload_uuid is None:
             # nothing was uploaded
             return
 
         log.info("finalizing inference upload for test run")
```

### Comparing `kolena_client-0.72.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.73.0/kolena/detection/_internal/test_suite.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,21 +41,21 @@
 from kolena.workflow._validators import assert_workflows_match
 
 
 class BaseTestSuite(ABC, Frozen, WithTelemetry):
     """
     A test suite groups together one or more test cases.
 
-    :param name: name of the test suite to create or load
-    :param version: optionally specify the version of the test suite to load. When absent, the latest version is loaded.
-        Ignored when creating new test suites
-    :param description: optionally specify a description for a newly created test suite. For existing test suites, this
-        description can be edited via :meth:`TestSuite.edit`
+    :param name: The name of the test suite to create or load.
+    :param version: Optionally specify the version of the test suite to load. When absent, the latest version is loaded.
+        Ignored when creating new test suites.
+    :param description: Optionally specify a description for a newly created test suite. For existing test suites, this
+        description can be edited via [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
     :param test_cases: optionally specify a list of test cases to populate a new test suite. For existing test suites,
-        test cases can be edited via :meth:`TestSuite.edit`
+        test cases can be edited via [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
     """
 
     _id: int
     _workflow: WorkflowType
 
     @classmethod
     @abstractmethod
@@ -159,39 +159,40 @@
         name: str,
         description: Optional[str] = None,
         test_cases: Optional[List[BaseTestCase]] = None,
     ) -> "BaseTestSuite":
         """
         Create a new test suite with the provided name.
 
-        :param name: the name of the new test suite to create.
-        :param description: optional free-form description of the test suite to create.
-        :param test_cases: optionally specify a set of test cases to populate the test suite.
-        :return: the newly created test suite.
+        :param name: The name of the new test suite to create.
+        :param description: Optional free-form description of the test suite to create.
+        :param test_cases: Optionally specify a set of test cases to populate the test suite.
+        :return: The newly created test suite.
         """
         return cls._create(cls._workflow, name, description, test_cases)
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "BaseTestSuite":
         """
         Load an existing test suite with the provided name.
 
-        :param name: the name of the test suite to load.
-        :param version: optionally specify a particular version of the test suite to load. Defaults to the latest
+        :param name: The name of the test suite to load.
+        :param version: Optionally specify a particular version of the test suite to load. Defaults to the latest
             version when unset.
-        :return: the loaded test suite.
+        :return: The loaded test suite.
         """
         data = cls._load_by_name(name, version)
         obj = cls._create_from_data(data)
         log.info(f"loaded test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         return obj
 
     class Editor:
         """
-        Interface to edit a test suite. Create with :meth:`TestSuite.edit`.
+        Interface to edit a test suite. Create with
+        [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
         """
 
         _test_cases: List[BaseTestCase]
         _reset: bool
         _description: str
         _initial_test_case_ids: Set[int]
         _initial_description: str
@@ -207,50 +208,54 @@
             self._initial_description = description
 
         @validate_arguments(config=ValidatorConfig)
         def description(self, description: str) -> None:
             """
             Update the description of the test suite.
 
-            :param description: the new description of the test suite
+            :param description: The new description of the test suite.
             """
             self._description = description
 
         @validate_arguments(config=ValidatorConfig)
         def add(self, test_case: BaseTestCase) -> None:
             """
-            Add the provided :class:`kolena.detection.TestCase` to the test suite.
+            Add the provided [`TestCase`][kolena.detection.TestCase] to the test suite.
             If a different version of the test case already exists in this test suite, it is replaced.
 
-            :param test_case: the test case to add to the test suite
+            :param test_case: The test case to add to the test suite.
             """
             self._assert_workflows_match(test_case)
             self._test_cases[test_case.name] = test_case._id
 
         @validate_arguments(config=ValidatorConfig)
         def remove(self, test_case: BaseTestCase) -> None:
             """
-            Remove the provided :class:`kolena.detection.TestCase` from the test suite. Any version of this test
+            Remove the provided [`TestCase`][kolena.detection.TestCase] from the test suite. Any version of this test
             case in this test suite will be removed; the version does not need to match exactly.
 
-            :param test_case: the test case to be removed from the test suite
+            :param test_case: The test case to be removed from the test suite.
             """
             name = test_case.name
             if name not in self._test_cases.keys():
                 raise KeyError(f"test case '{name}' not in test suite")
             self._test_cases.pop(name)
 
-        @deprecated(details="use :meth:`add` instead", deprecated_in="0.56.0")
+        @deprecated(details="use `TestSuite.Editor.add`", deprecated_in="0.56.0")
         @validate_arguments(config=ValidatorConfig)
         def merge(self, test_case: BaseTestCase) -> None:
             """
-            Add the provided :class:`kolena.detection.TestCase` to the test suite, replacing any previous version
+            !!! warning "Deprecated: since `0.56.0`"
+                Replaced by idempotent behavior in
+                [`TestSuite.Editor.add`][kolena.detection._internal.test_suite.BaseTestSuite.Editor.add].
+
+            Add the provided [`TestCase`][kolena.detection.TestCase] to the test suite, replacing any previous version
             of the test case that may be present in the suite.
 
-            :param test_case: the test case to be merged into the test suite
+            :param test_case: The test case to be merged into the test suite.
             """
             self.add(test_case)
 
         def _assert_workflows_match(self, test_case: BaseTestCase) -> None:
             if test_case._workflow != self._workflow:
                 raise ValueError(
                     f"test case workflow '{test_case._workflow}' mismatches test suite workflow '{self._workflow}'",
@@ -261,24 +266,26 @@
             return self._description != self._initial_description or self._initial_test_case_ids != test_case_ids
 
     @contextmanager
     def edit(self, reset: bool = False) -> Iterator[Editor]:
         """
         Edit this test suite in a context:
 
-        .. code-block:: python
-
-            with test_suite.edit() as editor:
-                # perform as many editing actions as desired
-                editor.add(...)
-                editor.remove(...)
-
-        Changes are committed to the Kolena platform when the context is exited.
-
-        :param reset: clear any and all test cases currently in the test suite.
+        ```python
+        with test_suite.edit() as editor:
+            # perform as many editing actions as desired
+            editor.add(...)
+            editor.remove(...)
+        ```
+
+        Changes are committed to Kolena when the context is exited.
+
+        :param reset: Clear any and all test cases currently in the test suite.
+        :return: Context-managed [`TestSuite.Editor`][kolena.detection._internal.test_suite.BaseTestSuite.Editor]
+            instance exposing editing functionality for this test suite.
         """
         editor = BaseTestSuite.Editor(self.test_cases, self.description, reset)
         editor._workflow = self._workflow  # set outside of init such that parameter does not leak into documentation
         if not reset:
             editor.description(self.description)
             for test_case in self.test_cases:
                 editor.add(test_case)
```

### Comparing `kolena_client-0.72.0/kolena/detection/ground_truth.py` & `kolena_client-0.73.0/kolena/detection/ground_truth.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,24 +28,19 @@
 from kolena.detection._internal.ground_truth import GroundTruthType
 
 
 class GroundTruth(Serializable, Frozen, metaclass=ABCMeta):
     """
     Base class for ground truths associated with an image.
 
-    See concrete implementations :class:`kolena.detection.ground_truth.ClassificationLabel`,
-    :class:`kolena.detection.ground_truth.BoundingBox`, :class:`kolena.detection.ground_truth.SegmentationMask`, for
-    details.
+    See concrete implementations [`BoundingBox`][kolena.detection.ground_truth.BoundingBox] and
+    [`SegmentationMask`][kolena.detection.ground_truth.SegmentationMask] for details.
     """
 
-    #: Label associated with this ground truth.
     label: str
-
-    #: A ground truth marked as `difficult' indicates that the object is considered difficult to recognize,
-    #: and should be ignored when evaluating metrics.
     difficult: bool
 
     @abstractmethod
     def __init__(self) -> None:
         ...
 
     @classmethod
@@ -67,24 +62,17 @@
                 label=data_object["label"],
                 points=data_object["points"],
                 difficult=data_object["difficult"],
             )
         raise ValueError(f"invalid dictionary provided, unrecognized data type '{data_type}'")
 
 
+# NOTE: intentionally leave undocumented; not a part of the public API
 class ClassificationLabel(GroundTruth):
-    """
-    Ground truth object representing a classification label.
-    """
-
-    #: Classification label to associate with the test sample.
     label: str
-
-    #: A classification label marked as `difficult' indicates that the object is considered difficult to recognize,
-    #: and should be ignored when evaluating metrics.
     difficult: bool
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, label: str, difficult: bool = False):
         super().__init__()
         validate_label(label)
         self.label = label
@@ -97,29 +85,31 @@
         )
 
 
 class BoundingBox(GroundTruth):
     """
     Ground truth data object representing a bounding box.
 
-    Point coordinates should be in (x, y) format, as absolute pixel values.
+    Point coordinates should be in `(x, y)` format, as absolute pixel values.
     """
 
-    #: Label to associate with this bounding box.
     label: str
+    """Label to associate with this bounding box."""
 
-    #: Point in (x, y) pixel coordinates representing the top left corner of the bounding box.
     top_left: Tuple[float, float]
+    """Point in `(x, y)` pixel coordinates representing the top left corner of the bounding box."""
 
-    #: Point in (x, y) pixel coordinates representing the bottom right corner of the bounding box.
     bottom_right: Tuple[float, float]
+    """Point in `(x, y)` pixel coordinates representing the bottom right corner of the bounding box."""
 
-    #: A bounding box marked as `difficult' indicates that the object is considered difficult to recognize,
-    #: and should be ignored when evaluating metrics.
     difficult: bool
+    """
+    A bounding box marked as `difficult` indicates that the object is considered difficult to recognize and should be
+    ignored when evaluating metrics.
+    """
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
         self,
         label: str,
         top_left: Tuple[float, float],
         bottom_right: Tuple[float, float],
@@ -139,29 +129,33 @@
         )
 
 
 class SegmentationMask(GroundTruth):
     """
     Ground truth data object representing a detection mask.
 
-    Point coordinates should be in (x, y) format, as absolute pixel values.
+    Point coordinates should be in `(x, y)` format, as absolute pixel values.
 
-    :raises ValueError: if fewer than three points are provided
+    :raises ValueError: When fewer than three points are provided.
     """
 
-    #: Label to associate with this segmentation mask.
     label: str
+    """Label to associate with this segmentation mask."""
 
-    #: Polygon corresponding to the vertices of the segmentation mask. Must have at least three distinct elements, and
-    #: may not cross itself or touch itself at any point.
     points: List[Tuple[float, float]]
+    """
+    Polygon corresponding to the vertices of the segmentation mask. Must have at least three distinct elements, and
+    may not cross itself or touch itself at any point.
+    """
 
-    #: A segmentation mask marked as `difficult' indicates that the object is considered difficult to recognize,
-    #: and should be ignored when evaluating metrics.
     difficult: bool
+    """
+    A segmentation mask marked as `difficult` indicates that the object is considered difficult to recognize and should
+    be ignored when evaluating metrics.
+    """
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, label: str, points: List[Tuple[float, float]], difficult: bool = False):
         super().__init__()
         validate_label(label)
         validate_polygon(points)
         self.label = label
```

### Comparing `kolena_client-0.72.0/kolena/detection/inference.py` & `kolena_client-0.73.0/kolena/detection/inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 from kolena._utils.inference_validators import validate_label
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import Inference as _Inference
 from kolena.detection._internal import InferenceType
 
 
 class Inference(_Inference):
+    """
+    Base class for model inferences associated with an image.
+
+    See concrete implementations [`BoundingBox`][kolena.detection.inference.BoundingBox], and
+    [`SegmentationMask`][kolena.detection.inference.SegmentationMask] for details.
+    """
+
     @classmethod
     def _from_dict(cls, ground_truth: Dict[str, Any]) -> "Inference":
         data_type = ground_truth["data_type"]
         data_object = ground_truth["data_object"]
         if data_type == InferenceType.CLASSIFICATION_LABEL.value:
             return ClassificationLabel(label=data_object["label"], confidence=data_object["confidence"])
         if data_type == InferenceType.BOUNDING_BOX.value:
@@ -46,23 +53,17 @@
                 label=data_object["label"],
                 confidence=data_object["confidence"],
                 points=data_object["points"],
             )
         raise ValueError(f"invalid dictionary provided, unrecognized data type '{data_type}'")
 
 
+# NOTE: intentionally leave undocumented; not a part of the public API
 class ClassificationLabel(Inference):
-    """
-    Inference representing a classification label.
-    """
-
-    #: Predicted classification label.
     label: str
-
-    #: Confidence score associated with this inference.
     confidence: float
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, label: str, confidence: float):
         validate_label(label)
         validate_confidence(confidence)
         self.label = label
@@ -75,28 +76,28 @@
         )
 
 
 class BoundingBox(Inference):
     """
     Inference representing a bounding box.
 
-    Point coordinates should be in (x, y) format, as absolute pixel values.
+    Point coordinates should be in `(x, y)` format, as absolute pixel values.
     """
 
-    #: Label to associate with this bounding box.
     label: str
+    """Label to associate with this bounding box."""
 
-    #: Confidence score associated with this inference.
     confidence: float
+    """Confidence score associated with this inference."""
 
-    #: Point in (x, y) pixel coordinates representing the top left corner of the bounding box.
     top_left: Tuple[float, float]
+    """Point in `(x, y)` pixel coordinates representing the top left corner of the bounding box."""
 
-    #: Point in (x, y) pixel coordinates representing the bottom right corner of the bounding box.
     bottom_right: Tuple[float, float]
+    """Point in `(x, y)` pixel coordinates representing the bottom right corner of the bounding box."""
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, label: str, confidence: float, top_left: Tuple[float, float], bottom_right: Tuple[float, float]):
         validate_label(label)
         validate_confidence(confidence)
         self.label = label
         self.confidence = confidence
@@ -110,28 +111,30 @@
         )
 
 
 class SegmentationMask(Inference):
     """
     Inference data object representing a segmentation mask.
 
-    Point coordinates should be in (x, y) format, as absolute pixel values.
+    Point coordinates should be in `(x, y)` format, as absolute pixel values.
 
-    :raises ValueError: if fewer than three points are provided
+    :raises ValueError: When fewer than three points are provided.
     """
 
-    #: Label to associate with this segmentation mask.
     label: str
+    """Label to associate with this segmentation mask."""
 
-    #: Confidence score associated with this inference.
     confidence: float
+    """Confidence score associated with this inference."""
 
-    #: Polygon corresponding to the vertices of the segmentation mask. Must have at least three distinct elements, and
-    #: may not cross itself or touch itself at any point.
     points: List[Tuple[float, float]]
+    """
+    Polygon corresponding to the vertices of the segmentation mask. Must have at least three distinct elements, and
+    may not cross itself or touch itself at any point.
+    """
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, label: str, confidence: float, points: List[Tuple[float, float]]):
         validate_label(label)
         validate_confidence(confidence)
         validate_polygon(points)
         self.label = label
```

### Comparing `kolena_client-0.72.0/kolena/detection/model.py` & `kolena_client-0.73.0/kolena/detection/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,28 @@
 from kolena.detection._internal import BaseModel
 from kolena.detection.inference import BoundingBox
 from kolena.detection.inference import SegmentationMask
 
 
 class Model(BaseModel):
     """
-    The descriptor for your model within the Kolena platform.
+    The descriptor for an object detection model within Kolena.
+
+    For additional functionality, see the associated
+    [base class documentation][kolena.detection._internal.model.BaseModel].
     """
 
-    #: Unique name of the model within the platform. If the provided model name has already been registered, that model
-    #: and its metadata are loaded upon instantiation.
     name: str
+    """
+    Unique name of the model within the platform. If the provided model name has already been registered, that model
+    and its metadata are loaded upon instantiation.
+    """
 
-    #: Unstructured metadata associated with the model.
     metadata: Dict[str, Any]
+    """Unstructured metadata associated with the model."""
 
     _TestImageClass = TestImage
     _TestCaseClass = TestCase
     _TestSuiteClass = TestSuite
     _InferenceClass = BoundingBox
     _LoadInferencesDataFrameClass = LoadInferencesDataFrame
 
@@ -57,20 +62,24 @@
         inferences = [Inference._from_dict(d) for d in record.inferences]
         bboxes = [inference for inference in inferences if isinstance(inference, (BoundingBox, SegmentationMask))]
         return test_image, bboxes
 
 
 class InferenceModel(Model):
     """
-    Extension of :class:`kolena.detection.Model` with custom ``infer`` method to perform inference.
+    Extension of [`Model`][kolena.detection.Model] with an `infer` method to perform inference.
+
+    See documentation parent [`Model`][kolena.detection.Model] for details.
     """
 
-    #: Function transforming a :class:`kolena.detection.TestImage` into a list of zero or more
-    #: :class:`kolena.detection.Inference` objects.
     infer: Callable[[TestImage], Optional[List[Inference]]]
+    """
+    Function transforming a [`TestImage`][kolena.detection.TestImage] into a list of zero or more
+    [`Inference`][kolena.detection.Inference] objects.
+    """
 
     def __init__(
         self,
         name: str,
         infer: Callable[[TestImage], Optional[List[Inference]]],
         metadata: Optional[Dict[str, Any]] = None,
     ):
```

### Comparing `kolena_client-0.72.0/kolena/detection/test_case.py` & `kolena_client-0.73.0/kolena/detection/test_case.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,22 +23,25 @@
 from kolena.detection._internal import BaseTestCase
 
 
 class TestCase(BaseTestCase):
     """
     A test case holds a set of images to compute performance metrics against.
 
-    :param name: name of the test case to create or load
-    :param version: optionally specify the version of the test case to load. When absent, the latest version is loaded.
-        Ignored when creating new test cases
-    :param description: optionally specify a description for a newly created test case. For existing test cases, this
-        description can be edited via :meth:`kolena.detection.TestCase.edit`
-    :param images: optionally provide a list of images and associated ground truths to populate a new test case. For
-        existing test cases, images can be edited via :meth:`kolena.detection.TestCase.edit`. Images must be registered
-        ahead of time with :meth:`kolena.detection.register_dataset`
+    For additional functionality, see the associated
+    [base class documentation][kolena.detection._internal.test_case.BaseTestCase].
+
+    :param name: Name of the test case to create or load.
+    :param version: Optionally specify the version of the test case to load. When absent, the latest version is loaded.
+        Ignored when creating new test cases.
+    :param description: Optionally specify a description for a newly created test case. For existing test cases, this
+        description can be edited via [`TestCase.edit`][kolena.detection._internal.test_case.BaseTestCase.edit].
+    :param images: Optionally provide a list of images and associated ground truths to populate a new test case. For
+        existing test cases, images can be edited via
+        [`TestCase.edit`][kolena.detection._internal.test_case.BaseTestCase.edit].
     """
 
     _TestImageClass = TestImage
     _TestImageDataFrameClass = TestImageDataFrame
 
     _workflow = WorkflowType.DETECTION
```

### Comparing `kolena_client-0.72.0/kolena/detection/test_config.py` & `kolena_client-0.73.0/kolena/detection/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,31 +13,38 @@
 # limitations under the License.
 from kolena._api.v1.detection import Metrics
 from kolena.detection._internal import TestConfig as _TestConfig
 from kolena.errors import InputValidationError
 
 
 class TestConfig(_TestConfig):
-    pass
+    """
+    Base class for testing configurations.
+
+    See concrete implementations [`FixedGlobalThreshold`][kolena.detection.FixedGlobalThreshold] and
+    [`F1Optimal`][kolena.detection.F1Optimal] for details.
+    """
 
 
 class FixedGlobalThreshold(TestConfig):
     """
-    Test configuration that sets the default display threshold in the Kolena UI to be a fixed global threshold for all
-    label classes within the test run.
+    Test configuration that sets the default display threshold in Kolena to a fixed global threshold for all classes
+    within the test suit.
     """
 
-    # The threshold used as the default for all label classes when visualizing results in the Kolena UI.
-    # Must be between 0 and 1.
     fixed_threshold: float
+    """
+    The threshold used as the default for all classes when visualizing results in Kolena. Must be between 0 and 1.
+    """
 
-    # The minimum intersection over union score between an inference and a ground truth for it to qualify as a potential
-    # match.
-    # Must be between 0 and 1.
     iou_threshold: float
+    """
+    The minimum intersection over union (IoU) score between an inference and a ground truth for it to qualify as a
+    potential match. Must be between 0 and 1.
+    """
 
     def __init__(self, fixed_threshold: float, iou_threshold: float = 0.5):
         if iou_threshold < 0 or iou_threshold > 1:
             raise InputValidationError(f"iou_threshold of {iou_threshold} was not between 0 and 1")
         if fixed_threshold < 0 or fixed_threshold > 1:
             raise InputValidationError(f"threshold of {fixed_threshold} was not between 0 and 1")
 
@@ -50,24 +57,25 @@
             iou_threshold=self.iou_threshold,
             params=dict(threshold=self.threshold),
         )
 
 
 class F1Optimal(TestConfig):
     """
-    Test configuration that sets the default display threshold in the Kolena UI to be dynamically set to the threshold
-    that corresponds to the highest F1 score for the test suite within the test run.
+    Test configuration that sets the default display threshold in Kolena to the threshold that corresponds to the
+    highest F1 score across all images within the test suite.
 
-    This threshold is evaluated and set per label for test suites with multiple label classes.
+    This threshold is evaluated and set per class for test suites with multiple classes.
     """
 
-    # The minimum intersection over union score between an inference and a ground truth for it to qualify as a potential
-    # match.
-    # Must be between 0 and 1.
     iou_threshold: float
+    """
+    The minimum intersection over union (IoU) score between an inference and a ground truth for it to qualify as a
+    potential match. Must be between 0 and 1.
+    """
 
     def __init__(self, iou_threshold: float = 0.5):
         if iou_threshold < 0 or iou_threshold > 1:
             raise InputValidationError(f"iou_threshold of {iou_threshold} was not between 0 and 1")
         self.iou_threshold = iou_threshold
 
     def _to_run_config(self) -> Metrics.RunConfig:
```

### Comparing `kolena_client-0.72.0/kolena/detection/test_image.py` & `kolena_client-0.73.0/kolena/detection/test_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,25 @@
 
 
 class TestImage(BaseTestImage):
     """
     Test image comprising a single image locator.
     """
 
-    #: List of :class:`kolena.detection.GroundTruth` labels associated with this image
+    locator: str
+    """Bucket locator for the provided test sample, e.g. `gs://my-bucket/path/to/image.png`."""
+
+    dataset: str
+    """Dataset this test image belongs to. Empty when unspecified."""
+
+    metadata: Dict[str, MetadataElement]
+    """Metadata associated with this test image. Surfaced during test runs."""
+
     ground_truths: List[GroundTruth]
+    """List of [`GroundTruth`][kolena.detection.ground_truth.GroundTruth] annotations associated with this image."""
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
         self,
         locator: str,
         dataset: Optional[str] = None,
         ground_truths: Optional[List[GroundTruth]] = None,
@@ -54,17 +63,17 @@
         super().__init__(locator, dataset, metadata)
         self.ground_truths = ground_truths or []
 
     def filter(self, predicate: Callable[[GroundTruth], bool]) -> "TestImage":
         """
         Return a copy of this test image with ground truths filtered to only those that match the provided predicate.
 
-        :param predicate: function accepting a :class:`kolena.detection.GroundTruth` and returning a boolean indicating
-            whether or not to include the ground truth
-        :return: a new test image with ground truths filtered by the predicate
+        :param predicate: Function accepting a [`GroundTruth`][kolena.detection.ground_truth.GroundTruth] and returning
+            a boolean indicating whether or not to include the ground truth.
+        :return: A new test image with ground truths filtered by the predicate.
         """
         return TestImage(**{**self._fields(), "ground_truths": [gt for gt in self.ground_truths if predicate(gt)]})
 
     @classmethod
     def _meta_keys(cls) -> List[str]:
         return ["locator", "dataset", "ground_truths", "metadata"]
 
@@ -89,35 +98,41 @@
         } == {**other.__dict__, "ground_truths": self._sort_ground_truths(other.ground_truths)}
 
     @staticmethod
     def _sort_ground_truths(ground_truths: List[GroundTruth]) -> List[GroundTruth]:
         return sorted(ground_truths, key=lambda gt: json.dumps(gt._to_dict(), sort_keys=True))
 
 
-@deprecated(details="use :class:`kolena.detection.TestCase.load_images`", deprecated_in="0.26.0")
+@deprecated(details="use `TestCase.load_images`", deprecated_in="0.26.0")
 @validate_arguments(config=ValidatorConfig)
 def load_images(dataset: Optional[str] = None) -> List[TestImage]:
     """
-    Load a list of :class:`kolena.detection.TestImage` samples registered in the Kolena platform.
+    !!! warning "Deprecated: since `0.26.0`"
+        Please use [`TestCase.load_images`][kolena.detection._internal.test_case.BaseTestCase.load_images] instead.
 
-    :param dataset: optionally specify the single dataset to be retrieved. By default, images from all
-        datasets are returned
+    Load a list of [`TestImage`][kolena.detection.TestImage] samples registered in Kolena.
+
+    :param dataset: Optionally specify the single dataset to be retrieved. By default, images from all
+        datasets are returned.
     """
     return list(iter_images(dataset))
 
 
-@deprecated(details="use :class:`kolena.detection.TestCase.iter_images`", deprecated_in="0.26.0")
+@deprecated(details="use `TestCase.iter_images`", deprecated_in="0.26.0")
 @validate_arguments(config=ValidatorConfig)
 def iter_images(dataset: Optional[str] = None) -> Iterator[TestImage]:
     """
-    Return iterator over :class:`kolena.detection.TestImage` samples registered in the Kolena platform. Images are
-    lazily loaded in chunks to facilitate working with large datasets that are cumbersome to hold in memory.
+    !!! warning "Deprecated: since `0.26.0`"
+        Please use [`TestCase.iter_images`][kolena.detection._internal.test_case.BaseTestCase.iter_images] instead.
+
+    Return iterator over [`TestImage`][kolena.detection.TestImage] samples registered in Kolena. Images are lazily
+    loaded in chunks to facilitate working with large datasets that are cumbersome to hold in memory.
 
-    :param dataset: optionally specify the single dataset to be retrieved. By default, images from all
-        datasets are returned
+    :param dataset: Optionally specify the single dataset to be retrieved. By default, images from all
+        datasets are returned.
     """
     init_request = API.InitLoadImagesRequest(dataset=dataset, batch_size=BatchSize.LOAD_RECORDS.value)
     for df in _BatchedLoader.iter_data(
         init_request=init_request,
         endpoint_path=API.Path.INIT_LOAD_IMAGES.value,
         df_class=TestImageDataFrame,
     ):
```

### Comparing `kolena_client-0.72.0/kolena/detection/test_run.py` & `kolena_client-0.73.0/kolena/detection/test_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,29 +31,30 @@
 from kolena.detection._internal.test_run import CustomMetricsCallback
 from kolena.detection.inference import Inference
 from kolena.detection.test_config import F1Optimal
 
 
 class TestRun(BaseTestRun):
     """
-    Interface to run tests for a :class:`kolena.detection.Model` on a set of :class:`kolena.detection.TestSuite` suites.
+    Interface to run tests for a [`Model`][kolena.detection.Model] on a [`TestSuite`][kolena.detection.TestSuite].
 
-    For a streamlined interface, see :meth:`kolena.detection.test`.
+    For a streamlined interface, see [`test`][kolena.detection.test].
 
-    Changes are committed to the Kolena platform during execution and when the context is exited.
+    Changes are committed to Kolena during execution and when the context is exited.
 
-    :param model: the model being tested.
-    :param test_suite: the test suite on which to test the model.
-    :param test_config: Optionally specify a :class:`kolena.detection.TestConfig` to customize the metrics
-                           evaluation logic for this test run. Defaults to :class:`kolena.detection.config.F1Optimal`
-                           with an iou_threshold of 0.5 if unspecified.
-    :param custom_metrics_callback: Optionally specify a callback function to compute custom metrics for each test-case.
-                                        The callback would be passed inferences of images in each testcase and should
-                                        return a dictionary with metric name as key and metric value as value.
-    :param reset: overwrites existing inferences if set.
+    :param model: The model being tested.
+    :param test_suite: The test suite on which to test the model.
+    :param test_config: Optionally specify a configuration, e.g.
+        [`FixedGlobalThreshold`][kolena.detection.FixedGlobalThreshold] to customize the metrics evaluation logic for
+        this test run. Defaults to [`F1Optimal`][kolena.detection.F1Optimal] with an `iou_threshold` of 0.5 if
+        unspecified.
+    :param custom_metrics_callback: Optionally specify a callback function to compute custom metrics for each test case.
+        The callback would be passed inferences of images in each testcase and should return a dictionary with metric
+        name as key and metric value as value.
+    :param reset: Overwrites existing inferences if set.
     """
 
     _TestImageClass = TestImage
     _InferenceClass = Inference
     _ImageResultDataFrameClass: Type[ImageResultDataFrame] = ImageResultDataFrame
     _LoadTestImagesDataFrameClass: Type[LoadTestImagesDataFrame] = LoadTestImagesDataFrame
 
@@ -90,28 +91,26 @@
     model: InferenceModel,
     test_suite: TestSuite,
     test_config: Optional[TestConfig] = None,
     custom_metrics_callback: Optional[CustomMetricsCallback[TestImage, Inference]] = None,
     reset: bool = False,
 ) -> None:
     """
-    Test the provided :class:`kolena.detection.InferenceModel` on one or more provided
-    :class:`kolena.detection.TestSuite` suites. Any tests already in progress for this model on these suites are
-    resumed.
-
-    :param model: the model being tested.
-    :param test_suite: the test suite on which to test the model.
-    :param test_config: Optionally specify a :class:`kolena.detection.TestConfig` to customize the metrics
-                           evaluation logic for this test run.
-                           Defaults to :class:`kolena.detection.test_config.F1Optimal` with an iou_threshold of 0.5
-                           if unspecified.
-    :param custom_metrics_callback: Optionally specify a callback function to compute custom metrics for each test-case.
-                                        The callback would be passed inferences of images in each testcase and should
-                                        return a dictionary with metric name as key and metric value as value.
-    :param reset: overwrites existing inferences if set.
+    Test the provided [`InferenceModel`][kolena.detection.InferenceModel] on the provided
+    [`TestSuite`][kolena.detection.TestSuite]. Any tests already in progress for this model on these suites are resumed.
+
+    :param model: The model to test.
+    :param test_suite: The test suite on which to test the model.
+    :param test_config: Optionally specify a configuration, e.g.
+        [`FixedGlobalThreshold`][kolena.detection.FixedGlobalThreshold], to customize metrics evaluation logic for this
+        test run. Defaults to [`F1Optimal`][kolena.detection.F1Optimal] with an `iou_threshold` of 0.5 if unspecified.
+    :param custom_metrics_callback: Optionally specify a callback function to compute custom metrics for each test case.
+        The callback would be passed inferences of images in each testcase and should return a dictionary with metric
+        name as key and metric value as value.
+    :param reset: Overwrites existing inferences if set.
     """
     with TestRun(
         model,
         test_suite,
         test_config=test_config,
         custom_metrics_callback=custom_metrics_callback,
         reset=reset,
```

### Comparing `kolena_client-0.72.0/kolena/detection/test_suite.py` & `kolena_client-0.73.0/kolena/detection/test_suite.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,35 +20,43 @@
 from kolena.detection._internal import BaseTestSuite
 
 
 class TestSuite(BaseTestSuite):
     """
     A test suite groups together one or more test cases.
 
-    :param name: name of the test suite to create or load
-    :param version: optionally specify the version of the test suite to load. When absent, the latest version is loaded.
-        Ignored when creating new test suites
-    :param description: optionally specify a description for a newly created test suite. For existing test suites, this
-        description can be edited via :meth:`TestSuite.edit`
-    :param test_cases: optionally specify a list of test cases to populate a new test suite. For existing test suites,
-        test cases can be edited via :meth:`TestSuite.edit`
+    For additional functionality, see the associated
+    [base class documentation][kolena.detection._internal.test_suite.BaseTestSuite].
+
+    :param name: Name of the test suite to create or load.
+    :param version: Optionally specify the version of the test suite to load. When absent, the latest version is loaded.
+        Ignored when creating new test suites.
+    :param description: Optionally specify a description for a newly created test suite. For existing test suites, this
+        description can be edited via [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
+    :param test_cases: Optionally specify a list of test cases to populate a new test suite. For existing test suites,
+        test cases can be edited via [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
     """
 
-    #: Unique name for this test suite. Cannot be changed after creation.
     name: str
+    """Unique name for this test suite."""
 
-    #: The version of the test suite. Each time the suite is edited with :meth:`kolena.detection.TestSuite.edit` the
-    #: version is automatically incremented.
     version: int
+    """
+    The version of the test suite. This version is automatically incremented each time the suite is edited with
+    [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
+    """
 
-    #: Free-form, human-readable description of the test suite. Can be edited at any time via :meth:`TestSuite.edit`.
     description: str
+    """
+    Free-form, human-readable description of the test suite. Can be edited at any time via
+    [`TestSuite.edit`][kolena.detection._internal.test_suite.BaseTestSuite.edit].
+    """
 
-    #: The test cases within the suite.
     test_cases: List[TestCase]
+    """The test cases within this test suite."""
 
     _id: int
     _workflow: WorkflowType = WorkflowType.DETECTION
 
     def __init__(
         self,
         name: str,
```

### Comparing `kolena_client-0.72.0/kolena/errors.py` & `kolena_client-0.73.0/kolena/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+Reference for various exceptions raised from `kolena`. All custom exceptions extend the base
+[`KolenaError`][kolena.errors.KolenaError].
+"""
 from requests import HTTPError
 
 
 class KolenaError(Exception):
     """Base error for all Kolena errors to extend. Allows consumers to catch Kolena specific errors."""
```

### Comparing `kolena_client-0.72.0/kolena/fr/__init__.py` & `kolena_client-0.73.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/fr/_utils.py` & `kolena_client-0.73.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/fr/datatypes.py` & `kolena_client-0.73.0/kolena/fr/datatypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+Schema declarations for the [Pandas DataFrames](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) used
+in `kolena.fr`.
+"""
 import json
 from typing import Any
 from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -135,43 +139,49 @@
 
 
 def _from_json(value: Optional[str]) -> Optional[Any]:
     return json.loads(value) if value is not None else None
 
 
 class TestImageDataFrameSchema(pa.SchemaModel):
-    # internal ID corresponding to this image
     image_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
+    """Internal ID corresponding to this image."""
 
-    # external locator pointing to image in bucket
     locator: Series[pa.typing.String] = pa.Field(coerce=True, _validate_locator=())
+    """External locator pointing to image in bucket."""
 
-    # specify source dataset, e.g. "CIFAR-10"
     data_source: Series[pa.typing.String] = pa.Field(coerce=True, nullable=True)
+    """Specify source dataset, e.g. "CIFAR-10"."""
 
-    # -1 used to specify "unspecified"
     width: Series[pa.typing.Int64] = pa.Field(coerce=True, _validate_optional_dimension=())
+    """Width of the image, in pixels. The value `-1` is used to specify "unspecified"."""
+
     height: Series[pa.typing.Int64] = pa.Field(coerce=True, _validate_optional_dimension=())
+    """Height of the image, in pixels. The value `-1` is used to specify "unspecified"."""
 
-    # specify that this image is an augmented version of another (registered) image
     original_locator: Series[pa.typing.String] = pa.Field(coerce=True, nullable=True, _validate_locator=())
+    """Specify that this image is an augmented version of another (registered) image."""
 
-    # free-form specification describing the augmentation applied to the image, e.g. {"rotate": 90}
-    # should not be specified unless original_locator is present
     augmentation_spec: Series[JSONObject] = pa.Field(coerce=True, nullable=True, _validate_json_object=())
+    """
+    Free-form specification describing the augmentation applied to the image, e.g. `{"rotate": 90}`. Should not be
+    specified unless original_locator is present.
+    """
 
-    # ground truth bounding box -- if absent, no ground truth will be available for display
     bounding_box: Series[BoundingBox] = pa.Field(coerce=True, nullable=True, _validate_bounding_box=())
+    """Ground truth bounding box. If absent, no ground truth will be available for display."""
 
-    # ground truth landmarks -- if absent, no ground truth will be available for display
     landmarks: Series[Landmarks] = pa.Field(coerce=True, nullable=True, _validate_landmarks=())
+    """Ground truth landmarks. If absent, no ground truth will be available for display."""
 
-    # specify a set of tags to apply to this object in the form {category: value}
-    # note that this format intentionally restricts tags to a single value per category
     tags: Series[JSONObject] = pa.Field(coerce=True, _validate_tags=())
+    """
+    Specify a set of tags to apply to this object in the form `{category: value}`. Note that this format
+    intentionally restricts tags to a single value per category.
+    """
 
 
 TestImageRecord = Tuple[
     str,
     Optional[str],
     int,
     int,
@@ -206,48 +216,58 @@
 
 class ImageDataFrameSchema(pa.SchemaModel):
     image_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
     locator: Series[pa.typing.String] = pa.Field(coerce=True)
 
 
 class ImageResultDataFrameSchema(pa.SchemaModel):
-    #: [**Required**] The ID of the image corresponding to this record.
     image_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
+    """[**Required**] The ID of the image corresponding to this record."""
 
-    #: [Optional] A bounding box around the face detected in this image.
     bounding_box: Optional[Series[BoundingBox]] = pa.Field(coerce=True, nullable=True, _validate_bounding_box=())
+    """[Optional] A bounding box around the face detected in this image."""
 
-    #: [Optional] RGB image (``np.ndarray`` with cells of type ``np.uint8``) corresponding to the input to the
-    #: "landmarks" model in the face recognition pipeline.
     landmarks_input_image: Optional[Series[RGBImage]] = pa.Field(coerce=True, nullable=True, _validate_rgb_image=())
+    """
+    [Optional] RGB image (`np.ndarray` with cells of type `np.uint8`) corresponding to the input to the "landmarks"
+    model in the face recognition pipeline.
+    """
 
-    #: [Optional] A 10-element array with ``(x, y)`` coordinates corresponding to the left eye, right eye, nose tip,
-    #: left mouth corner, right mouth corner of the detected face.
     landmarks: Optional[Series[Landmarks]] = pa.Field(coerce=True, nullable=True, _validate_landmarks=())
+    """
+    [Optional] A 10-element array with `(x, y)` coordinates corresponding to the left eye, right eye, nose tip, left
+    mouth corner, right mouth corner of the detected face.
+    """
 
-    #: [Optional] RGB image (``np.ndarray`` with cells of type ``np.uint8``) corresponding to the input to the "quality"
-    #: model in the face recognition pipeline.
     quality_input_image: Optional[Series[RGBImage]] = pa.Field(coerce=True, nullable=True, _validate_rgb_image=())
+    """
+    [Optional] RGB image (`np.ndarray` with cells of type `np.uint8`) corresponding to the input to the "quality" model
+    in the face recognition pipeline.
+    """
 
-    #: [Optional] Score produced by the "quality" model in the face recognition pipeline.
     quality: Optional[Series[pa.typing.Float64]] = pa.Field(coerce=True, nullable=True)
+    """[Optional] Score produced by the "quality" model in the face recognition pipeline."""
 
-    #: [Optional] Score produced by the "acceptability" model in the face recognition pipeline.
     acceptability: Optional[Series[pa.typing.Float64]] = pa.Field(coerce=True, nullable=True)
+    """[Optional] Score produced by the "acceptability" model in the face recognition pipeline."""
 
-    #: [Optional] RGB image (``np.ndarray`` with cells of type ``np.uint8``) corresponding to the input to the facial
-    #: embeddings extraction model in the face recognition pipeline.
     fr_input_image: Optional[Series[RGBImage]] = pa.Field(coerce=True, nullable=True, _validate_rgb_image=())
+    """
+    [Optional] RGB image (`np.ndarray` with cells of type `np.uint8`) corresponding to the input to the facial
+    embeddings extraction model in the face recognition pipeline.
+    """
 
-    #: [Optional] Embedding vector (``np.ndarray``) extracted representing the face detected in the image. An empty cell
-    #: (no array is provided) indicates a failure to enroll for the image, i.e. no face detected.
     embedding: Series[EmbeddingVector] = pa.Field(coerce=True, nullable=True, _validate_embedding_vector=())
+    """
+    [Optional] Embedding vector (`np.ndarray`) extracted representing the face detected in the image. An empty cell
+    (no array is provided) indicates a failure to enroll for the image, i.e. no face detected.
+    """
 
-    #: [Optional] The reason why the image was a failure to enroll.
     failure_reason: Optional[Series[pa.typing.String]] = pa.Field(coerce=True, nullable=True)
+    """[Optional] The reason why the image was a failure to enroll."""
 
 
 class _ResultStageFrameSchema(pa.SchemaModel):
     test_run_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
     image_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
     # null values for the following columns indicate a failure to enroll
     bbox: Series[pa.typing.String] = pa.Field(coerce=True, nullable=True)
@@ -264,46 +284,55 @@
     key: Series[pa.typing.String] = pa.Field(coerce=True)
     uuid: Series[pa.typing.String] = pa.Field(coerce=True)
     image: Series[RGBImage] = pa.Field(coerce=True, _validate_rgb_image=())
 
 
 class EmbeddingDataFrameSchema(pa.SchemaModel):
     image_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
+    """The provided ID of the image."""
 
-    #: The extracted embedding(s) corresponding to the ``image_id``. A missing embedding indicates a failure to enroll
-    #: for the image.
-    #:
-    #: For images with only one extracted embedding, the ``embedding`` is a one-dimensional ``np.ndarray`` with length
-    #: matching the length of the extracted embedding. When multiple embeddings were extracted from a single image, the
-    #: first dimension represents the index of the extracted embedding. For example, for an image with 3 extracted
-    #: embeddings and embeddings of length 256, the ``embedding`` is an array of shape (3, 256).
     embedding: Series[EmbeddingVector] = pa.Field(nullable=True, coerce=True, _validate_embedding_vector=())
+    """
+    The extracted embedding(s) corresponding to the `image_id`. A missing embedding indicates a failure to enroll
+    for the image.
+
+    For images with only one extracted embedding, the `embedding` is a one-dimensional `np.ndarray` with length
+    matching the length of the extracted embedding. When multiple embeddings were extracted from a single image, the
+    first dimension represents the index of the extracted embedding. For example, for an image with 3 extracted
+    embeddings and embeddings of length 256, the `embedding` is an array of shape (3, 256).
+    """
 
 
 class PairDataFrameSchema(pa.SchemaModel):
     image_pair_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
     image_a_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
     image_b_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
 
 
 class PairResultDataFrameSchema(pa.SchemaModel):
-    #: [**Required**] The ID of the image corresponding to this record.
     image_pair_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
+    """[**Required**] The ID of the image corresponding to this record."""
 
-    #: [Optional] The similarity score computed between the two embeddings in this image pair. Should be left empty when
-    #: either image in the pair is a failure to enroll.
     similarity: Series[pa.typing.Float64] = pa.Field(nullable=True, coerce=True)
+    """
+    [Optional] The similarity score computed between the two embeddings in this image pair. Should be left empty when
+    either image in the pair is a failure to enroll.
+    """
 
-    #: [Optional] Index of the embedding in ``image_a`` corresponding to this similarity score. Required when multiple
-    #: embeddings are extracted per image and multiple similarity scores are computed per image pair.
     embedding_a_index: Optional[Series[pa.typing.Int64]] = pa.Field(nullable=True, coerce=True)
+    """
+    [Optional] Index of the embedding in `image_a` corresponding to this similarity score. Required when multiple
+    embeddings are extracted per image and multiple similarity scores are computed per image pair.
+    """
 
-    #: [Optional] Index of the embedding in ``image_b`` corresponding to this similarity score. Required when multiple
-    #: embeddings are extracted per image and multiple similarity scores are computed per image pair.
     embedding_b_index: Optional[Series[pa.typing.Int64]] = pa.Field(nullable=True, coerce=True)
+    """
+    [Optional] Index of the embedding in `image_b` corresponding to this similarity score. Required when multiple
+    embeddings are extracted per image and multiple similarity scores are computed per image pair.
+    """
 
 
 class LoadedPairResultDataFrameSchema(TestCaseDataFrameSchema, PairResultDataFrameSchema):  # note inheritance
     image_a_fte: Series[pa.typing.Bool] = pa.Field(coerce=True)  # if image_a failed to enroll (FTE)
     image_b_fte: Series[pa.typing.Bool] = pa.Field(coerce=True)  # if image_b failed to enroll (FTE)
```

### Comparing `kolena_client-0.72.0/kolena/fr/model.py` & `kolena_client-0.73.0/kolena/fr/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,45 +37,43 @@
 
 
 class Model(Uninstantiable["Model.Data"]):
     """The descriptor for your model within the Kolena platform."""
 
     @dataclass(frozen=True, config=ValidatorConfig)
     class Data:
-        """The data stored for your model in the platform."""
-
         id: int
         name: str
         metadata: Dict[str, Any]
 
     @classmethod
     def create(cls, name: str, metadata: Dict[str, Any]) -> "Model":
         """
         Create a new model with the provided name and metadata.
 
-        :param name: unique name of the new model to create
-        :param metadata: unstructured metadata to associate with the model
-        :return: the created model
-        :raises ValueError: if a model by the provided name already exists
+        :param name: Unique name of the new model to create.
+        :param metadata: Unstructured metadata to associate with the model.
+        :return: The newly created model.
+        :raises ValueError: A model by the provided name already exists.
         """
         request = API.CreateRequest(name=name, metadata=metadata)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
         log.info(f"created model '{name}' ({get_model_url(obj.data.id)})")
         return obj
 
     @classmethod
     def load_by_name(cls, name: str) -> "Model":
         """
         Retrieve the existing model with the provided name.
 
-        :param name: name of the model to retrieve
-        :return: the retrieved model
-        :raises KeyError: if no model with the provided name exists
+        :param name: Name of the model to retrieve.
+        :return: The retrieved model.
+        :raises KeyError: If no model with the provided name exists.
         """
         request = API.LoadByNameRequest(name=name)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
         log.info(f"loaded model '{name}' ({get_model_url(obj.data.id)})")
         return obj
@@ -102,46 +100,47 @@
         """
         Load previously stored pair results for this model on the provided test case or test suite. If this model has
         not been run on the provided test object, a zero-length response is returned. Partial results are returned when
         testing on the requested test case or test suite is incomplete.
 
         The returned DataFrame has the following relevant fields:
 
-        - ``locator_a``: the locator pointing to the left image in the pair
-        - ``locator_b``: the locator pointing to the right image in the pair
-        - ``is_same``: boolean indicating if the two images depict the same person or a different person
-        - ``image_a_fte``: boolean indicating that the left image failed to enroll (FTE)
-        - ``image_b_fte``: boolean indicating that the right image failed to enroll (FTE)
-        - ``similarity``: float similarity score between the left and right images. ``NaN`` if either image failed to
+        - `locator_a`: the locator pointing to the left image in the pair
+        - `locator_b`: the locator pointing to the right image in the pair
+        - `is_same`: boolean indicating if the two images depict the same person or a different person
+        - `image_a_fte`: boolean indicating that the left image failed to enroll (FTE)
+        - `image_b_fte`: boolean indicating that the right image failed to enroll (FTE)
+        - `similarity`: float similarity score between the left and right images. `NaN` if either image failed to
           enroll. When multiple similarity scores were provided for a given image pair, only the highest similarity
           score is returned
 
-        :param test_object: the :class:`kolena.fr.TestSuite` or :class:`kolena.fr.TestCase` to load pair results from
-        :raises ValueError: if an invalid test object was provided
-        :raises RemoteError: if the pair results could not be loaded for any reason
+        :param test_object: The [`TestSuite`][kolena.fr.TestSuite] or [`TestCase`][kolena.fr.TestCase] to load pair
+            results from.
+        :raises ValueError: An invalid test object was provided.
+        :raises RemoteError: The pair results could not be loaded for any reason.
         """
         return _BatchedLoader.concat(self.iter_pair_results(test_object), LoadedPairResultDataFrame)
 
     def iter_pair_results(
         self,
         test_object: Union[TestSuite, TestSuite.Data, TestCase, TestCase.Data],
         batch_size: int = 10_000_000,
     ) -> Iterator[LoadedPairResultDataFrame]:
         """
         Iterator over DataFrames of previously stored pair results for this model on the provided test case or test
         suite, grouped in batches. If this model has not been run on the provided test object, a zero-length response
         is returned. Partial results are returned when testing on the requested test case or test suite is incomplete.
 
-        See :meth:`load_pair_results` for details on the returned DataFrame.
+        See [`Model.load_pair_results`][kolena.fr.Model.load_pair_results] for details on the returned DataFrame.
 
-        :param test_object: the :class:`kolena.fr.TestSuite` or :class:`kolena.fr.TestCase` to load pair results from
-        :param batch_size: optionally specify maximum number of rows to be returned in a single DataFrame. By default,
-            limits row count to 10_000_000.
-        :raises ValueError: if an invalid test object was provided
-        :raises RemoteError: if the pair results could not be loaded for any reason
+        :param test_object: The [`TestSuite`][kolena.fr.TestSuite] or [`TestCase`][kolena.fr.TestCase] to load pair
+            results from.
+        :param batch_size: Optionally specify maximum number of rows to be returned in a single DataFrame.
+        :raises ValueError: An invalid test object was provided.
+        :raises RemoteError: The pair results could not be loaded for any reason.
         """
         display_type = "test case" if isinstance(test_object, (TestCase, TestCase.Data)) else "test suite"
         display_name = test_object.data.name if isinstance(test_object, (TestCase, TestSuite)) else test_object.name
         test_object_display_name = f"{display_type} '{display_name}'"
         log.info(f"loading pair results from model '{self.data.name}' on {test_object_display_name}")
         base_load_request = dataclasses.asdict(self._get_load_pair_results_request(test_object))
         init_request = API.InitLoadPairResultsRequest(batch_size=batch_size, **base_load_request)
@@ -151,41 +150,59 @@
             df_class=LoadedPairResultDataFrame,
         )
         log.info(f"loaded pair results from model '{self.data.name}' on {test_object_display_name}")
 
 
 class InferenceModel(Model):
     """
-    A :class:`kolena.fr.Model` capable of running tests via :meth:`kolena.fr.test`.
+    A [`Model`][kolena.fr.Model] capable of running tests via [`test`][kolena.fr.test].
 
     Currently supports extracting a single embedding per image. To extract multiple embeddings per image, see
-    :meth:`kolena.fr.TestRun`.
+    [`TestRun`][kolena.fr.TestRun].
     """
 
     extract: Callable[[str], Optional[np.ndarray]]
     compare: Callable[[np.ndarray, np.ndarray], float]
 
     @classmethod
     def create(
         cls,
         name: str,
         extract: Callable[[str], Optional[np.ndarray]],
         compare: Callable[[np.ndarray, np.ndarray], float],
         metadata: Dict[str, Any],
     ) -> "InferenceModel":
+        """
+        Create a new model with the provided name and metadata.
+
+        :param name: Unique name of the new model to create.
+        :param extract: A function implementing embeddings extraction for this model.
+        :param compare: A function implementing embeddings similarity comparison for this model.
+        :param metadata: Unstructured metadata to associate with the model.
+        :return: The newly created model.
+        :raises ValueError: A model by the provided name already exists.
+        """
         base_model = super().create(name, metadata)
         return cls._from_base(base_model, extract, compare)
 
     @classmethod
     def load_by_name(
         cls,
         name: str,
         extract: Callable[[str], Optional[np.ndarray]],
         compare: Callable[[np.ndarray, np.ndarray], float],
     ) -> "InferenceModel":
+        """
+        Load an existing model.
+
+        :param name: The name of the model to load.
+        :param extract: A function implementing embeddings extraction for this model.
+        :param compare: A function implementing embeddings similarity comparison for this model.
+        :return: The loaded model.
+        """
         base_model = super().load_by_name(name)
         return cls._from_base(base_model, extract, compare)
 
     @staticmethod
     def _from_base(
         base_model: Model,
         extract: Callable[[str], Optional[np.ndarray]],
```

### Comparing `kolena_client-0.72.0/kolena/fr/test_case.py` & `kolena_client-0.73.0/kolena/fr/test_case.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,39 +42,43 @@
 from kolena.fr.datatypes import TestCaseDataFrame
 from kolena.fr.datatypes import TestCaseDataFrameSchema
 from kolena.fr.datatypes import TestCaseRecord
 
 
 class TestCase(ABC, Frozen, WithTelemetry):
     """
-    A group of test samples that can be added to a :class:`kolena.fr.TestSuite`.
+    A group of image pairs that can be added to a [`TestSuite`][kolena.fr.TestSuite].
 
     The test case is the base unit of results computation in the Kolena platform. Metrics are computed by test case.
     """
 
-    #: The unique name of this test case. Cannot be changed after creation.
     name: str
+    """The unique name of this test case. Cannot be changed after creation."""
 
-    #: The version of this test case. A test case's version is automatically incremented whenever it is edited via
-    #: :meth:`TestCase.edit`.
     version: int
+    """
+    The version of this test case. A test case's version is automatically incremented whenever it is edited via
+    [`TestCase.edit`][kolena.fr.TestCase.edit].
+    """
 
-    #: Free-form, human-readable description of this test case. Can be edited at any time via :meth:`TestCase.edit`.
     description: str
+    """
+    Free-form, human-readable description of this test case. Can be edited at any time via
+    [`TestCase.edit`][kolena.fr.TestCase.edit].
+    """
 
-    #: The count of images attached to this test case
     image_count: int
+    """The number of images included in this test case."""
 
-    #: The count of genuine image pairs attached to this test case
     pair_count_genuine: int
+    """The number of genuine image pairs included in this test case."""
 
-    #: The count of imposter image pairs attached to this test case
     pair_count_imposter: int
+    """The number of imposter image pairs included in this test case."""
 
-    #: Deprecated, use :class:`kolena._api.v1.fr.TestCase.EntityData` instead
     Data = API.EntityData
 
     _id: int
     _data: API.EntityData
 
     def __init__(
         self,
@@ -96,37 +100,43 @@
         except NotFoundError:
             if version is not None:
                 log.warn(f"creating new test case '{name}', ignoring provided version")
             self._populate_from_other(self.create(name, description, test_samples))
         self._freeze()
 
     @property
-    @deprecated(details="use values on :class:`kolena.fr.TestCase` directly", deprecated_in="0.57.0")
+    @deprecated(details="use `TestCase` instance attributes", deprecated_in="0.57.0")
     def data(self) -> API.EntityData:
+        """
+        !!! warning "Deprecated: since `0.57.0`"
+            Access this data via instance attributes, e.g. `self.image_count`, directly.
+
+        The data associated with this test case.
+        """
         return self._data
 
     @data.setter
-    @deprecated(details="use values on :class:`kolena.fr.TestCase` directly", deprecated_in="0.57.0")
+    @deprecated(details="use `TestCase` instance attributes", deprecated_in="0.57.0")
     def data(self, new_data: API.EntityData) -> None:
         self._data = new_data
 
     @classmethod
     def create(
         cls,
         name: str,
         description: Optional[str] = None,
         test_samples: Optional[List[TestCaseRecord]] = None,
     ) -> "TestCase":
         """
         Create a new test case with the provided name.
 
-        :param name: the name of the new test case to create.
-        :param description: optional free-form description of the test case to create.
-        :param test_samples: optionally specify a set of test samples to populate the test case.
-        :return: the newly created test case.
+        :param name: The name of the new test case to create.
+        :param description: Optional free-form description of the test case to create.
+        :param test_samples: Optionally specify a set of test samples to populate the test case.
+        :return: The newly created test case.
         """
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test case '{name}' (v{obj.version})")
@@ -135,28 +145,31 @@
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
         Load an existing test case with the provided name.
 
-        :param name: the name of the test case to load.
-        :param version: optionally specify a particular version of the test case to load. Defaults to the latest version
+        :param name: The name of the test case to load.
+        :param version: Optionally specify a particular version of the test case to load. Defaults to the latest version
             when unset.
-        :return: the loaded test case.
+        :return: The loaded test case.
         """
         return cls._load_by_name(name, version)
 
     @classmethod
-    @deprecated(details="use :meth:`load` instead", deprecated_in="0.57.0")
+    @deprecated(details="use `TestCase.load`", deprecated_in="0.57.0")
     def load_by_name(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
+        !!! warning "Deprecated: since `0.57.0`"
+            Use [`TestCase.load`][kolena.fr.TestCase.load] instead.
+
         Load an existing test case with the provided name.
 
-        :param name: the name of the test case to load
+        :param name: The name of the test case to load.
         :param version: optionally specify the target version of the test case to load. When absent, the highest version
             of the test case with the provided name is returned
         :return: the loaded test case
         """
         return cls.load(name, version)
 
     @classmethod
@@ -166,17 +179,17 @@
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         log.info(f"loaded test case '{name}' (v{data.version})")
         return cls._create_from_data(data)
 
     def load_data(self) -> TestCaseDataFrame:
         """
-        Load all pairs data for a test case.
+        Load all image pairs for a test case.
 
-        :return: a DataFrame containing all pairs defined in this test case
+        :return: DataFrame containing all pairs defined in this test case.
         """
         return _BatchedLoader.concat(self.iter_data(), TestCaseDataFrame)
 
     @classmethod
     def _create_from_data(cls, data: API.EntityData) -> "TestCase":
         obj = cls.__new__(cls)
         obj._id = data.id
@@ -225,46 +238,45 @@
             self._samples: Dict[str, TestCaseRecord] = OrderedDict()
 
         @validate_arguments(config=ValidatorConfig)
         def description(self, description: str) -> None:
             """
             Update the description of this test case.
 
-            :param description: the new test case description
+            :param description: The new test case description.
             """
             self._description = description
 
         @validate_arguments(config=ValidatorConfig)
         def add(self, locator_a: str, locator_b: str, is_same: bool) -> None:
             """
             Add the provided image pair to the test case.
 
-            Note that if the image pair with ``locator_a`` and ``locator_b`` is already defined within the platform,
-            the value for ``is_same`` must match the value already defined.
+            Note that if the image pair with `locator_a` and `locator_b` is already defined within the platform,
+            the value for `is_same` must match the value already defined.
 
-            :param locator_a: the left locator for the image pair
-            :param locator_b: the right locator for the image pair
-            :param is_same: whether or not these images should be considered a true pair or an imposter pair
-            :raises ValueError: the image pair already exists in the test case
+            :param locator_a: The left locator for the image pair.
+            :param locator_b: The right locator for the image pair.
+            :param is_same: Whether to treat this image pair as a a genuine pair (`True`) or an imposter pair (`False`).
             """
             key = self._key(locator_a, locator_b)
             val = (locator_a, locator_b, is_same)
             if val == self._samples.get(key, None):
                 log.info(f"no op: {val} already in test case")
                 return
             self._samples[key] = val
 
         @validate_arguments(config=ValidatorConfig)
         def remove(self, locator_a: str, locator_b: str) -> None:
             """
             Remove the provided pair from the test case.
 
-            :param locator_a: the left locator for the image pair
-            :param locator_b: the right locator for the image pair
-            :raises KeyError: if the provided locator pair is not in the test case
+            :param locator_a: The left locator for the image pair.
+            :param locator_b: The right locator for the image pair.
+            :raises KeyError: If the provided locator pair is not in the test case.
             """
             key = self._key(locator_a, locator_b)
             if key not in self._samples.keys():
                 raise KeyError(f"pair not in test case: {locator_a}, {locator_b}")
             self._samples.pop(key)
 
         @staticmethod
@@ -278,24 +290,24 @@
             )
 
     @contextmanager
     def edit(self, reset: bool = False) -> Iterator[Editor]:
         """
         Edit this test case in a context:
 
-        .. code-block:: python
-
-            with test_case.edit() as editor:
-                # perform as many editing actions as desired
-                editor.add(...)
-                editor.remove(...)
+        ```python
+        with test_case.edit() as editor:
+            # perform as many editing actions as desired
+            editor.add(...)
+            editor.remove(...)
+        ```
 
         Changes are committed to the Kolena platform when the context is exited.
 
-        :param reset: clear any and all test samples currently in the test case.
+        :param reset: Clear any and all test samples currently in the test case.
         """
         editor = self.Editor(self.description, reset)
 
         if not reset:
             df_existing = self.load_data()
             # avoid calling the expensive self.load_data() multiple times
             _initial_samples: Dict[str, TestCaseRecord] = OrderedDict()
@@ -335,16 +347,15 @@
         log.success(f"edited test case '{self.name}' (v{self.version})")
 
     @validate_arguments
     def iter_data(self, batch_size: int = 10_000_000) -> Iterator[TestCaseDataFrame]:
         """
         Iterator of DataFrames describing all pairs data for a test case.
 
-        :param batch_size: optionally specify maximum number of rows to be returned in a single DataFrame. By default,
-            limits row count to 10_000_000.
+        :param batch_size: Optionally specify maximum number of rows to be returned in a single DataFrame.
         """
         log.info(f"loading image pairs in test case '{self.name}' (v{self.version})")
         init_request = API.InitLoadDataRequest(batch_size=batch_size, test_case_id=self._id)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_DATA.value,
             df_class=TestCaseDataFrame,
```

### Comparing `kolena_client-0.72.0/kolena/fr/test_images.py` & `kolena_client-0.73.0/kolena/fr/test_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,19 +53,20 @@
         cls,
         data_source: Optional[Union[str, TestSuite, TestSuite.Data, TestCase, TestCase.Data]] = None,
         include_augmented: bool = False,
     ) -> TestImageDataFrame:
         """
         Load a DataFrame describing images registered in the Kolena platform.
 
-        :param data_source: optionally specify the single data source to be retrieved, e.g. ``"my-data-source"``.
-            Alternatively, provide a :class:`kolena.fr.TestSuite` or :class:`kolena.fr.TestCase` as source.
-            If no argument is provided, all images registered using :meth:`TestImages.register` are returned
-        :param include_augmented: optionally specify that augmented images should be returned. By default, only
-            original images are returned. Ignored when test case or test suite is provided as ``data_source``
+        :param data_source: Optionally specify the single data source to be retrieved, e.g. `"my-data-source"`.
+            Alternatively, provide a [`TestSuite`][kolena.fr.TestSuite] or [`TestCase`][kolena.fr.TestCase] as source.
+            If no argument is provided, all images registered using
+            [`TestImages.register][kolena.fr.TestImages.register] are returned.
+        :param include_augmented: Optionally specify that augmented images should be returned. By default, only
+            original images are returned. Ignored when test case or test suite is provided as `data_source`.
         """
         log.info("loading test images")
         return _BatchedLoader.concat(
             cls.iter(data_source=data_source, include_augmented=include_augmented),
             TestImageDataFrame,
         )
 
@@ -86,23 +87,23 @@
             landmarks: Optional[np.ndarray] = None,
             tags: Optional[Dict[str, str]] = None,
         ) -> None:
             """
             Add a new image to Kolena. If the provided locator is already registered with the platform, its metadata
             will be updated.
 
-            :param locator: bucket locator for the provided image, e.g. ``s3://bucket-name/path/to/image.jpg``
-            :param data_source: name of the source for the image being registered
-            :param width: width in pixels of the image being registered
-            :param height: height in pixels of the image being registered
-            :param bounding_box: optional 4-element array specifying the ground truth bounding box for this image, of
-                the form ``[top_left_x, top_left_y, bottom_right_x, bottom_right_y]``
-            :param landmarks: optional 10-element array specifying (x, y) coordinates for five facial landmarks of the
-                form ``[left_eye_{x,y}, right_eye_{x,y}, nose_{x,y}, left_mouth_{x,y}, right_mouth_{x,y}]``
-            :param tags: tags to associate with the image, of the form ``{category: value}``
+            :param locator: Bucket locator for the provided image, e.g. `s3://bucket-name/path/to/image.jpg`.
+            :param data_source: Name of the source for the image being registered.
+            :param width: Width in pixels of the image being registered.
+            :param height: Height in pixels of the image being registered.
+            :param bounding_box: Optional 4-element array specifying the ground truth bounding box for this image, of
+                the form `[top_left_x, top_left_y, bottom_right_x, bottom_right_y]`.
+            :param landmarks: Optional 10-element array specifying (x, y) coordinates for five facial landmarks of the
+                form `[left_eye_{x,y}, right_eye_{x,y}, nose_{x,y}, left_mouth_{x,y}, right_mouth_{x,y}]`.
+            :param tags: Tags to associate with the image, of the form `{category: value}`.
             """
             if locator in self.data.locators:
                 raise ValueError(f"duplicate locator: {locator}")
             self.data.locators.add(locator)
             self.data.records.append(
                 (
                     locator,
@@ -131,26 +132,26 @@
         ) -> None:
             """
             Add an augmented version of an existing image to Kolena.
 
             Note that the original image must already be registered in a previous pass. Tags on the original image are
             not propagated forward to the augmented image.
 
-            :param original_locator: the bucket locator for the original version of this image within the platform
-            :param augmented_locator: the bucket locator for the augmented image being registered
-            :param augmentation_spec: free-form JSON specification for the augmentation applied to this image
-            :param width: optionally specify the width of the augmented image. When absent, the width of the
-                corresponding original image is used
-            :param height: optionally specify the height of the augmented image. When absent, the height of the
-                corresponding original image is used
-            :param bounding_box: optionally specify a new bounding box for the augmented image. When absent, any
-                bounding box corresponding to the original image is used
-            :param landmarks: optionally specify a new set of landmarks for the augmented image. When absent, any set of
-                landmarks corresponding to the original image is used
-            :param tags: optionally specify a set of tags to associate with the augmented image
+            :param original_locator: The bucket locator for the original version of this image within the platform.
+            :param augmented_locator: The bucket locator for the augmented image being registered.
+            :param augmentation_spec: Free-form JSON specification for the augmentation applied to this image.
+            :param width: Optionally specify the width of the augmented image. When absent, the width of the
+                corresponding original image is used.
+            :param height: Optionally specify the height of the augmented image. When absent, the height of the
+                corresponding original image is used.
+            :param bounding_box: Optionally specify a new bounding box for the augmented image. When absent, any
+                bounding box corresponding to the original image is used.
+            :param landmarks: Optionally specify a new set of landmarks for the augmented image. When absent, any set of
+                landmarks corresponding to the original image is used.
+            :param tags: Optionally specify a set of tags to associate with the augmented image.
             """
             if augmented_locator in self.data.locators:
                 raise ValueError(f"duplicate locator: {augmented_locator}")
             self.data.locators.add(augmented_locator)
             self.data.records.append(
                 (
                     augmented_locator,
@@ -168,15 +169,15 @@
     @classmethod
     @contextmanager
     def register(cls) -> Iterator[Registrar]:
         """
         Context-managed interface to register new images with Kolena. Images with locators that already exist in the
         platform will have their metadata updated. All changes are committed when the context is exited.
 
-        :raises RemoteError: if the registered images were unable to be successfully committed for any reason
+        :raises RemoteError: The registered images were unable to be successfully committed for any reason.
         """
         log.info("registering test images")
         registrar = TestImages.Registrar.__factory__(TestImages._Registrar(records=[], locators=set()))
         yield registrar
 
         init_response = init_upload()
         df = pd.DataFrame(registrar.data.records, columns=TEST_IMAGE_COLUMNS)
@@ -200,21 +201,21 @@
         data_source: Optional[Union[str, TestSuite, TestSuite.Data, TestCase, TestCase.Data]] = None,
         include_augmented: bool = False,
         batch_size: int = 10_000_000,
     ) -> Iterator[TestImageDataFrame]:
         """
         Iterator of DataFrames describing images registered in the Kolena platform.
 
-        :param data_source: optionally specify the single data source to be retrieved, e.g. ``"my-data-source"``.
-            Alternatively, provide a :class:`kolena.fr.TestSuite` or :class:`kolena.fr.TestCase` as source.
-            If no argument is provided, all images registered using :meth:`TestImages.register` are returned
-        :param include_augmented: optionally specify that augmented images should be returned. By default, only
-            original images are returned. Ignored when test case or test suite is provided as ``data_source``
-        :param batch_size: optionally specify maximum number of rows to be returned in a single DataFrame. By default,
-            limits row count to 10_000_000.
+        :param data_source: Optionally specify the single data source to be retrieved, e.g. `"my-data-source"`.
+            Alternatively, provide a [`TestSuite`][kolena.fr.TestSuite] or [`TestCase`][kolena.fr.TestCase] as source.
+            If no argument is provided, all images registered using
+            [`TestImages.register`][kolena.fr.TestImages.register] are returned.
+        :param include_augmented: Optionally specify that augmented images should be returned. By default, only
+            original images are returned. Ignored when test case or test suite is provided as `data_source`.
+        :param batch_size: Optionally specify maximum number of rows to be returned in a single DataFrame.
         """
         test_suite_data = data_source.data if isinstance(data_source, TestSuite) else data_source
         test_suite_id = test_suite_data.id if isinstance(test_suite_data, TestSuite.Data) else None
         test_case_data = data_source.data if isinstance(data_source, TestCase) else data_source
         test_case_id = test_case_data.id if isinstance(test_case_data, TestCase.Data) else None
         data_source_display_name = cls._data_source_display_name(data_source, include_augmented)
         from_extra = f" from '{data_source_display_name}'" if data_source_display_name is not None else ""
```

### Comparing `kolena_client-0.72.0/kolena/fr/test_run.py` & `kolena_client-0.73.0/kolena/fr/test_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,22 +53,22 @@
 from kolena.fr.datatypes import PairDataFrame
 from kolena.fr.datatypes import PairResultDataFrame
 from kolena.fr.datatypes import PairResultDataFrameSchema
 
 
 class TestRun(ABC, Frozen, WithTelemetry):
     """
-    Interface to run tests for a :class:`kolena.fr.Model` on a set of
-    :class:`kolena.fr.TestSuite` suites. Any in-progress tests for this model on these suites are resumed.
+    Interface to test a [`Model`][kolena.fr.Model] on a [`TestSuite`][kolena.fr.TestSuite]. Any in-progress tests for
+    this model on this test suite is resumed.
 
-    For a streamlined interface, see :meth:`kolena.fr.test`.
+    For a streamlined interface, see [`test`][kolena.fr.test].
 
-    :param model: the model being tested.
-    :param test_suite: the test suite on which to test the model.
-    :param reset: overwrites existing inferences if set.
+    :param model: The model being tested.
+    :param test_suite: The test suite on which to test the model.
+    :param reset: Overwrites existing inferences if set.
     """
 
     _id: int
 
     @dataclass(frozen=True, config=ValidatorConfig)
     class Data:
         id: int
@@ -93,37 +93,40 @@
         self._id = response.id
         self._model = model
         self._test_suite = test_suite
         self._reset = reset
         self._freeze()
 
     @classmethod
-    @deprecated(details="use initializer :class:`kolena.fr.TestRun` directly", deprecated_in="0.58.0")
+    @deprecated(details="use `TestRun.__init__` directly", deprecated_in="0.58.0")
     def create_or_retrieve(cls, model: Model, test_suite: TestSuite, reset: bool = False) -> "TestRun":
         """
-        Create a new test run for the provided :class:`kolena.fr.Model` on the provided :class:`kolena.fr.TestSuite`.
-        If a test run for this model on this suite already exists, it is returned.
+        !!! warning "Deprecated: since `0.57.0`"
+            Use the [`TestRun`][kolena.fr.TestRun] constructor instead.
 
-        :param model: the model being tested.
-        :param test_suite: the test suite on which to test the model.
-        :param reset: overwrites existing inferences if set.
-        :return: the created or retrieved test run.
+        Create a new test run for the provided [`Model`][kolena.fr.Model] on the provided
+        [`TestSuite`][kolena.fr.TestSuite]. If a test run for this model on this suite already exists, it is returned.
+
+        :param model: The model being tested.
+        :param test_suite: The test suite on which to test the model.
+        :param reset: Overwrites existing inferences if set.
+        :return: The created or retrieved test run.
         """
         return TestRun(model, test_suite, reset=reset)
 
     @validate_arguments
     def load_remaining_images(self, batch_size: int = 10_000_000) -> ImageDataFrame:
         """
         Load a DataFrame containing records for each of the images in the configured test suite that does not yet have
         results from the configured model.
 
-        :param batch_size: optionally specify the maximum number of image records to return. Defaults to ``10_000_000``.
+        :param batch_size: Optionally specify the maximum number of image records to return.
         :return: DataFrame containing records for each of the images that must be processed.
-        :raises InputValidationError: if the requested ``batch_size`` failed validation.
-        :raises RemoteError: if images could not be loaded for any reason.
+        :raises InputValidationError: The requested `batch_size` failed validation.
+        :raises RemoteError: Images could not be loaded for any reason.
         """
         if batch_size <= 0:
             raise InputValidationError(f"invalid batch_size '{batch_size}': expected positive integer")
         log.info("loading remaining images for test run")
         init_request = API.InitLoadRemainingImagesRequest(
             test_run_id=self.data.id,
             batch_size=batch_size,
@@ -148,26 +151,26 @@
             finally:
                 _BatchedLoader.complete_load(load_uuid)
 
     def upload_image_results(self, df_image_result: ImageResultDataFrame) -> int:
         """
         Upload inference results for a batch of images.
 
-        All columns except for ``image_id`` and ``embedding`` are optional. An empty ``embedding`` cell in a record
-        indicates a failure to enroll. The ``failure_reason`` column can optionally be specified for failures to enroll.
+        All columns except for `image_id` and `embedding` are optional. An empty `embedding` cell in a record
+        indicates a failure to enroll. The `failure_reason` column can optionally be specified for failures to enroll.
 
         To provide more than one embedding extracted from a given image, include multiple records with the same
-        ``image_id`` in ``df_image_result`` (one for each embedding extracted). Records for a given ``image_id`` must
-        be submitted in the same ``df_image_result`` DataFrame, and **not** across multiple calls to
-        ``upload_image_results``.
+        `image_id` in `df_image_result` (one for each embedding extracted). Records for a given `image_id` must
+        be submitted in the same `df_image_result` DataFrame, and **not** across multiple calls to
+        `upload_image_results`.
 
         :param df_image_result: DataFrame of any size containing records describing inference results for an image.
-        :return: number of records successfully uploaded.
-        :raises TypeValidationError: if the DataFrame failed type validation.
-        :raises RemoteError: if the DataFrame was unable to be successfully ingested for any reason.
+        :return: Number of records successfully uploaded.
+        :raises TypeValidationError: The DataFrame failed type validation.
+        :raises RemoteError: The DataFrame was unable to be successfully ingested for any reason.
         """
         log.info("uploading inference results for test run")
         init_response = init_upload()
 
         asset_config_res = krequests.get(endpoint_path=AssetAPI.Path.CONFIG.value)
         krequests.raise_for_status(asset_config_res)
         asset_config = from_dict(data_class=AssetAPI.Config, data=asset_config_res.json())
@@ -201,24 +204,24 @@
 
     @validate_arguments
     def load_remaining_pairs(self, batch_size: int = 10_000_000) -> Tuple[EmbeddingDataFrame, PairDataFrame]:
         """
         Load DataFrames containing computed embeddings and records for each of the image pairs in the configured test
         suite that have not yet had similarity scores computed.
 
-        This method should not be called until all images in the :class:`TestRun` have been processed.
+        This method should not be called until all images in the [`TestRun`][kolena.fr.TestRun] have been processed.
 
-        :param batch_size: optionally specify the maximum number of image pair records to return. Defaults to
-            ``10_000_000``.
-        :return: two DataFrames, one containing embeddings computed in the previous step (``df_embedding``) and one
-            containing records for each of the image pairs that must be computed (``df_pair``). See documentation on
-            :class:`kolena.fr.datatypes.EmbeddingDataFrameSchema` for expected format when multiple embeddings were
-            uploaded from a single image in :meth:`kolena.fr.TestRun.upload_image_results`.
-        :raises InputValidationError: if the requested ``batch_size`` failed validation.
-        :raises RemoteError: if pairs could not be loaded for any reason.
+        :param batch_size: Optionally specify the maximum number of image pair records to return.
+        :return: Two DataFrames, one containing embeddings computed in the previous step (`df_embedding`) and one
+            containing records for each of the image pairs that must be computed (`df_pair`). See documentation on
+            [`EmbeddingDataFrameSchema`][kolena.fr.datatypes.EmbeddingDataFrameSchema] for expected format when multiple
+            embeddings were uploaded from a single image in
+            [`TestRun.upload_image_results`][kolena.fr.TestRun.upload_image_results].
+        :raises InputValidationError: The requested `batch_size` failed validation.
+        :raises RemoteError: Pairs could not be loaded for any reason.
         """
         if batch_size <= 0:
             raise InputValidationError(f"invalid batch_size '{batch_size}': expected positive integer")
 
         log.info("loading batch of image pairs for test run")
         init_request = API.InitLoadRemainingPairsRequest(
             test_run_id=self.data.id,
@@ -257,30 +260,30 @@
 
     def upload_pair_results(self, df_pair_result: PairResultDataFrame) -> int:
         """
         Upload image pair similarity results for a batch of pairs.
 
         This method should not be called until all images in the TestRun have been processed.
 
-        All columns except for ``image_pair_id`` and ``similarity`` are optional. An empty ``similarity`` cell in a
+        All columns except for `image_pair_id` and `similarity` are optional. An empty `similarity` cell in a
         record indicates a pair failure (i.e. one or more of the images in the pair failed to enroll).
 
         For image pairs containing images with more than one embedding, a single record may be provided with the highest
-        similarity score, or ``M x N`` records may be provided for each embeddings combination in the pair, when there
-        are ``M`` embeddings from ``image_a`` and ``N`` embeddings from ``image_b``.
+        similarity score, or `M x N` records may be provided for each embeddings combination in the pair, when there
+        are `M` embeddings from `image_a` and `N` embeddings from `image_b`.
 
-        When providing multiple records for a given image pair, use the ``embedding_a_index`` and ``embedding_b_index``
+        When providing multiple records for a given image pair, use the `embedding_a_index` and `embedding_b_index`
         columns to indicate which embeddings were used to compute a given similarity score. Records for a given image
-        pair must be submitted in the same ``df_pair_result`` DataFrame, and **not** across multiple calls to
-        ``upload_pair_results``.
+        pair must be submitted in the same `df_pair_result` DataFrame, and **not** across multiple calls to
+        `upload_pair_results`.
 
         :param df_pair_result: DataFrame containing records describing the similarity score of a pair of images.
-        :return: number of records successfully uploaded.
-        :raises TypeValidationError: if the DataFrame failed type validation.
-        :raises RemoteError: if the DataFrame was unable to be successfully ingested for any reason.
+        :return: Number of records successfully uploaded.
+        :raises TypeValidationError: The DataFrame failed type validation.
+        :raises RemoteError: The DataFrame was unable to be successfully ingested for any reason.
         """
         log.info("uploading pair results for test run")
         init_response = init_upload()
 
         df_validated = validate_df_schema(df_pair_result, PairResultDataFrameSchema)
         validate_df_record_count(df_validated)
         upload_data_frame(df_validated, BatchSize.UPLOAD_RECORDS.value, init_response.uuid)
@@ -295,20 +298,20 @@
         response = from_dict(data_class=API.UploadPairResultsResponse, data=finalize_res.json())
         return response.n_uploaded
 
 
 @validate_arguments(config=ValidatorConfig)
 def test(model: InferenceModel, test_suite: TestSuite, reset: bool = False) -> None:
     """
-    Test the provided :class:`kolena.fr.InferenceModel` on one or more provided :class:`kolena.fr.TestSuite` suites. Any
-    tests already in progress for this model on these suites are resumed.
+    Test the provided [`InferenceModel`][kolena.fr.InferenceModel] on the provided [`TestSuite`][kolena.fr.TestSuite].
+    Any tests already in progress for this model on these suites are resumed.
 
-    :param model: the model being tested, implementing both ``extract`` and ``compare`` methods.
-    :param test_suite: the test suite on which to test the model.
-    :param reset: overwrites existing inferences if set.
+    :param model: The model being tested, implementing both `extract` and `compare` methods.
+    :param test_suite: The test suite on which to test the model.
+    :param reset: Overwrites existing inferences if set.
     """
     test_run = TestRun(model, test_suite, reset=reset)
 
     try:
         log.info("starting test run")
         df_image = test_run.load_remaining_images(int(1e12))
         df_image["embedding"] = [
```

### Comparing `kolena_client-0.72.0/kolena/fr/test_suite.py` & `kolena_client-0.73.0/kolena/fr/test_suite.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,40 +37,44 @@
 
 
 class TestSuite(ABC, Frozen, WithTelemetry):
     """
     A test suite groups together one or more test cases.
     """
 
-    #: The unique name of this test suite. Cannot be changed after creation.
     name: str
+    """The unique name of this test suite."""
 
-    #: The version of this test suite. A test suite's version is automatically incremented whenever it is edited via
-    #: :meth:`TestSuite.edit`.
     version: int
+    """
+    The version of this test suite. A test suite's version is automatically incremented whenever it is edited via
+    [`TestSuite.edit`][kolena.fr.TestSuite.edit].
+    """
 
-    #: Free-form, human-readable description of this test suite. Can be edited at any time via :meth:`TestSuite.edit`.
     description: str
+    """
+    Free-form, human-readable description of this test suite. Can be edited at any time via
+    [`TestSuite.edit`][kolena.fr.TestSuite.edit].
+    """
 
-    #: The baseline :class:`kolena.fr.TestCase` objects belonging to this test suite
     baseline_test_cases: List[TestCase]
+    """The baseline [`TestCase`][kolena.fr.TestCase] object(s) for this test suite."""
 
-    #: The non-baseline :class:`kolena.fr.TestCase` objects belonging to this test suite
     non_baseline_test_cases: List[TestCase]
+    """The non-baseline [`TestCase`][kolena.fr.TestCase] object(s) for this test suite."""
 
-    #: The count of images attached to the baseline test cases
     baseline_image_count: int
+    """The number of images attached to the baseline test case(s)."""
 
-    #: The count of genuine pair attached to the baseline test cases
     baseline_pair_count_genuine: int
+    """The number of genuine pairs attached to the baseline test case(s)."""
 
-    #: The count of imposter pair attached to the baseline test cases
     baseline_pair_count_imposter: int
+    """The count of imposter pairs attached to the baseline test case(s)."""
 
-    #: Deprecated, use :class:`kolena._api.v1.fr.TestSuite.EntityData` instead
     Data = API.EntityData
 
     _id: int
     _data: API.EntityData
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
@@ -94,38 +98,45 @@
         except NotFoundError:
             if version is not None:
                 log.warn(f"creating new test suite '{name}', ignoring provided version")
             self._populate_from_other(self.create(name, description, baseline_test_cases, non_baseline_test_cases))
         self._freeze()
 
     @property
-    @deprecated(details="use values on :class:`kolena.fr.TestSuite` directly", deprecated_in="0.57.0")
+    @deprecated(details="use `TestSuite` instance attributes", deprecated_in="0.57.0")
     def data(self) -> API.EntityData:
+        """
+        !!! warning "Deprecated: since `0.57.0`"
+            Access this data via instance attributes, e.g. `self.baseline_test_cases`, directly.
+
+        The data associated with this test suite.
+        """
         return self._data
 
     @data.setter
-    @deprecated(details="use values on :class:`kolena.fr.TestSuite` directly", deprecated_in="0.57.0")
+    @deprecated(details="use `TestSuite` instance attributes", deprecated_in="0.57.0")
     def data(self, new_data: API.EntityData) -> None:
         self._data = new_data
 
     @classmethod
     def create(
         cls,
         name: str,
         description: Optional[str] = None,
         baseline_test_cases: Optional[List[TestCase]] = None,
         non_baseline_test_cases: Optional[List[TestCase]] = None,
     ) -> "TestSuite":
         """
         Create a new test suite with the provided name.
 
-        :param name: the name of the new test suite to create.
-        :param description: optional free-form description of the test suite to create.
-        :param test_cases: optionally specify a set of test cases to populate the test suite.
-        :return: the newly created test suite.
+        :param name: The name of the new test suite to create.
+        :param description: Optional free-form description of the test suite to create.
+        :param baseline_test_cases: Optionally specify a list of test cases to use as baseline for the test suite.
+        :param non_baseline_test_cases: Optionally specify a list of test cases to populate the test suite.
+        :return: The newly created test suite.
         """
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
@@ -141,24 +152,27 @@
         :param version: optionally specify a particular version of the test suite to load. Defaults to the latest
             version when unset.
         :return: the loaded test suite.
         """
         return cls._load_by_name(name, version)
 
     @classmethod
-    @deprecated(details="use :meth:`load` instead", deprecated_in="0.57.0")
+    @deprecated(details="use `TestSuite.load`", deprecated_in="0.57.0")
     def load_by_name(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         """
+        !!! warning "Deprecated: since `0.57.0`"
+            Use [`TestSuite.load`][kolena.fr.TestSuite.load] instead.
+
         Retrieve the existing test suite with the provided name.
 
-        :param name: name of the test suite to retrieve.
-        :param version: optionally specify the version of the named test suite to retrieve. When absent the latest
+        :param name: Name of the test suite to retrieve.
+        :param version: Optionally specify the version of the named test suite to retrieve. When absent the latest
             version of the test suite is returned.
-        :return: the retrieved test suite.
-        :raises NotFoundError: if the test suite with the provided name doesn't exist.
+        :return: The retrieved test suite.
+        :raises NotFoundError: If the test suite with the provided name doesn't exist.
         """
         return cls.load(name, version)
 
     @classmethod
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         request = API.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
@@ -209,17 +223,15 @@
                 for test_case in baseline_test_cases:
                     editor.add(test_case, True)
             if non_baseline_test_cases is not None:
                 for test_case in non_baseline_test_cases:
                     editor.add(test_case, False)
 
     class Editor:
-        """
-        Interface to edit a test suite. Create with :meth:`TestSuite.edit`.
-        """
+        """Interface to edit a test suite. Create with [`TestSuite.edit`][kolena.fr.TestSuite.edit]."""
 
         _edited: bool
         _reset: bool
         _description: str
         _initial_description: str
         _baseline_test_cases: Dict[str, int]
         _non_baseline_test_cases: Dict[str, int]
@@ -234,28 +246,28 @@
             self._edited = False
 
         @validate_arguments(config=ValidatorConfig)
         def description(self, description: str) -> None:
             """
             Update the description of the test suite.
 
-            :param description: the new description of the test suite
+            :param description: The new description of the test suite.
             """
             self._description = description
             self._edited = True
 
         @validate_arguments(config=ValidatorConfig)
         def add(self, test_case: TestCase, is_baseline: Optional[bool] = None) -> None:
             """
             Add a test case to this test suite. If a different version of the test case already exists in this test
-            suite, it is replaced and its baseline status will be propagated when is_baseline is unset.
+            suite, it is replaced and its baseline status will be propagated when `is_baseline` is unset.
 
-            :param test_case: the test case to add to the test suite.
-            :param is_baseline: specify that this test case is a part of the "baseline," i.e. if the samples in this
-                test case should contribute to the computation of thresholds within this test suite
+            :param test_case: The test case to add to the test suite.
+            :param is_baseline: Specify that this test case is a part of the "baseline," i.e. if the samples in this
+                test case should contribute to the computation of thresholds within this test suite.
             """
             name = test_case.name
             # clean up any previous versions and propagates its baseline status
             set_is_baseline: Optional[bool] = None
             if name in self._baseline_test_cases.keys():
                 self._baseline_test_cases.pop(name)
                 set_is_baseline = is_baseline if is_baseline is not None else True
@@ -265,38 +277,41 @@
 
             is_baseline_ret = set_is_baseline or is_baseline or False
             self._add(test_case, is_baseline=is_baseline_ret)
 
         @validate_arguments(config=ValidatorConfig)
         def remove(self, test_case: TestCase) -> None:
             """
-            Remove the provided :class:`kolena.fr.TestCase` from the test suite. Any version of this test case in the
-            suite will be removed; the version does not need to match exactly.
+            Remove the provided [`TestCase`][kolena.fr.TestCase] from the test suite. Any version of this test case in
+            the suite will be removed; the version does not need to match exactly.
 
-            :param test_case: the test case to be removed
+            :param test_case: The test case to remove.
             """
             name = test_case.name
             if name in self._baseline_test_cases.keys():
                 self._baseline_test_cases.pop(name)
             elif name in self._non_baseline_test_cases.keys():
                 self._non_baseline_test_cases.pop(name)
             else:
                 raise KeyError(f"test case '{name}' not in test suite")
             self._edited = True
 
-        @deprecated(details="use :meth:`add` instead", deprecated_in="0.57.0")
+        @deprecated(details="use `TestSuite.Editor.add`", deprecated_in="0.57.0")
         @validate_arguments(config=ValidatorConfig)
         def merge(self, test_case: TestCase, is_baseline: Optional[bool] = None) -> None:
             """
-            Add the :class:`kolena.fr.TestCase` to the suite. If a test case by this name already exists in the suite,
-            replace the previous version of that test case with the newly provided version.
+            !!! warning "Deprecated: since `0.57.0`"
+                Replaced by idempotent behavior in [`TestSuite.Editor.add`][kolena.fr.TestSuite.Editor.add].
+
+            Add the [`TestCase`][kolena.fr.TestCase] to the suite. If a test case by this name already exists in the
+            suite, replace the previous version of that test case with the newly provided version.
 
-            :param test_case: the test case to be merged into the test suite
-            :param is_baseline: optionally specify whether or not this test case should be considered as a part of the
-                baseline for this test suite. When not specified, the previous value for ``is_baseline`` for this test
+            :param test_case: The test case to be merged into the test suite.
+            :param is_baseline: Optionally specify whether or not this test case should be considered as a part of the
+                baseline for this test suite. When not specified, the previous value for `is_baseline` for this test
                 case in this test suite is propagated forward. Defaults to false if the test case does not already exist
                 in this suite.
             """
             self.add(test_case, is_baseline)
 
         @validate_arguments(config=ValidatorConfig)
         def _add(self, test_case: TestCase, is_baseline: bool = False) -> None:
@@ -308,14 +323,19 @@
             self._edited = True
 
     @contextmanager
     def edit(self, reset: bool = False) -> Iterator[Editor]:
         """
         Context-managed way to perform many modification options on a test suite and commit the results when the context
         is exited, resulting in a single version bump.
+
+        ```python
+        with TestSuite.load("my-test-suite").edit() as editor:
+            editor.add(TestCase.load("my-test-case"))
+        ```
         """
         editor = TestSuite.Editor(self.description, reset)
         if not reset:
             for baseline_test_case in self.baseline_test_cases:
                 editor.add(baseline_test_case, is_baseline=True)
             for non_baseline_test_case in self.non_baseline_test_cases:
                 editor.add(non_baseline_test_case, is_baseline=False)
```

### Comparing `kolena_client-0.72.0/kolena/initialize.py` & `kolena_client-0.73.0/kolena/initialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,28 +32,39 @@
     verbose: bool = False,
     proxies: Optional[Dict[str, str]] = None,
     **kwargs: Any,
 ) -> None:
     """
     Initialize a client session.
 
+    Retrieve an API token from [app.kolena.io/~/developer](https://app.kolena.io/redirect/developer) and
+    populate the `KOLENA_TOKEN` environment variable before initializing:
+
+    ```python
+    import os
+    import kolena
+
+    kolena.initialize(os.environ["KOLENA_TOKEN"], verbose=True)
+    ```
+
     A session has a global scope and remains active until interpreter shutdown.
 
-    .. note:: As of version 0.29.0: the entity param is no longer needed; ``initialize(entity, token)`` is
-        **deprecated** and replaced by ``initialize(token)``.
+    !!! note
+        As of version 0.29.0: the `entity` argument is no longer needed; the signature `initialize(entity, api_token)`
+        has been deprecated and replaced by `initialize(api_token)`.
 
-    :param api_token: provided API token. This token is a secret and should be treated with caution
-    :param verbose: optionally configure client to run in verbose mode, providing more information about execution. All
-        logging events are emitted as Python standard library ``logging`` events from the ``"kolena"`` logger as well as
-        to stdout/stderr directly
-    :param proxies: optionally configure client to run with ``http`` or ``https`` proxies. The ``proxies`` parameter
-        is passed through to the ``requests`` package and can be
-        `configured accordingly <https://requests.readthedocs.io/en/latest/user/advanced/#proxies>`_
-    :raises InvalidTokenError: the provided ``api_token`` is not valid
-    :raises InputValidationError: the provided combination or number of args is not valid
+    :param api_token: Provided API token. This token is a secret and should be treated with caution.
+    :param verbose: Optionally configure client to run in verbose mode, providing more information about execution. All
+        logging events are emitted as Python standard library `logging` events from the `"kolena"` logger as well as
+        to stdout/stderr directly.
+    :param proxies: Optionally configure client to run with `http` or `https` proxies. The `proxies` parameter
+        is passed through to the `requests` package and can be
+        [configured accordingly](https://requests.readthedocs.io/en/latest/user/advanced/#proxies).
+    :raises InvalidTokenError: The provided `api_token` is not valid.
+    :raises InputValidationError: The provided combination or number of args is not valid.
     """
     used_deprecated_signature = False
 
     if len(args) > 1:
         raise InputValidationError(f"Too many args. Expected 0 or 1 but got {len(args)} Check docs for usage.")
     elif len(args) == 1:
         # overwrite the originally passed api_token since we are supporting backward compatability with entity
```

### Comparing `kolena_client-0.72.0/kolena/workflow/_datatypes.py` & `kolena_client-0.73.0/kolena/workflow/_datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 from kolena._utils.validators import ValidatorConfig
 
 T = TypeVar("T", bound="DataObject")
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class DataObject(metaclass=ABCMeta):
+    """The base for various objects in `kolena.workflow`."""
+
     def _to_dict(self) -> Dict[str, Any]:
         def serialize_value(value: Any) -> Any:
             if isinstance(value, (bool, str, int, float)) or value is None:
                 return value
             if isinstance(value, np.generic):  # numpy scalars are common enough to be worth specific handling
                 for base_type, numpy_type in [(bool, np.bool_), (int, np.integer), (float, np.inexact)]:
                     if isinstance(value, numpy_type):  # cast if there is a match, otherwise fallthrough
```

### Comparing `kolena_client-0.72.0/kolena/workflow/_helpers.py` & `kolena_client-0.73.0/kolena/workflow/define_workflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,28 +33,48 @@
     test_sample_type: Type[TestSample],
     ground_truth_type: Type[GroundTruth],
     inference_type: Type[Inference],
 ) -> Tuple[Workflow, Type[TestCase], Type[TestSuite], Type[Model]]:
     """
     Define a new workflow, specifying its test sample, ground truth, and inference types.
 
-    Provided as a convenience method to create the :class:`TestCase`, :class:`TestSuite`, and :class:`Model` objects
-    for a new workflow. These objects can also be defined manually by subclassing them and binding the ``workflow``
+    ```python
+    from kolena.workflow import define_workflow
+
+    from my_code import MyTestSample, MyGroundTruth, MyInference
+
+    _, TestCase, TestSuite, Model = define_workflow(
+        "My Workflow",
+        MyTestSample,   # extends e.g. kolena.workflow.Image (or uses directly)
+        MyGroundTruth,  # extends kolena.workflow.GroundTruth
+        MyInference,    # extends kolena.workflow.Inference
+    )
+    ```
+
+    `define_workflow` is provided as a convenience method to create the [`TestCase`][kolena.workflow.TestCase],
+    [`TestSuite`][kolena.workflow.TestSuite], and [`Model`][kolena.workflow.Model] objects
+    for a new workflow. These objects can also be defined manually by subclassing them and binding the `workflow`
     class variable:
 
-    .. code-block:: python
+    ```python
+    from kolena.workflow import TestCase
 
-        from kolena.workflow import TestCase
-        from my_code import my_workflow
+    from my_code import my_workflow
 
-        class MyTestCase(TestCase):
-            workflow = my_workflow
+    class MyTestCase(TestCase):
+        workflow = my_workflow
+    ```
 
-    :return: the :class:`Workflow` object for this workflow along with the :class:`TestCase`, :class:`TestSuite`,
-        and :class:`Model` objects to use when creating and running tests for this workflow.
+    :param name: The name of the workflow.
+    :param test_sample_type: The type of the [`TestSample`][kolena.workflow.TestSample] for this workflow.
+    :param ground_truth_type: The type of the [`GroundTruth`][kolena.workflow.GroundTruth] for this workflow.
+    :param inference_type: The type of the [`Inference`][kolena.workflow.Inference] for this workflow.
+    :return: The `Workflow` object for this workflow along with the [`TestCase`][kolena.workflow.TestCase],
+        [`TestSuite`][kolena.workflow.TestSuite], and [`Model`][kolena.workflow.Model] objects to use when creating and
+        running tests for this workflow.
     """
     workflow = Workflow(
         name=name,
         test_sample_type=test_sample_type,
         ground_truth_type=ground_truth_type,
         inference_type=inference_type,
     )
```

### Comparing `kolena_client-0.72.0/kolena/workflow/_validators.py` & `kolena_client-0.73.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.72.0/kolena/workflow/annotation.py` & `kolena_client-0.73.0/kolena/workflow/annotation.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,34 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+Annotations are visualized in Kolena as overlays on top of [`TestSample`][kolena.workflow.TestSample] objects.
+
+The following annotation types are available:
+
+- [`BoundingBox`][kolena.workflow.annotation.BoundingBox]
+- [`Polygon`][kolena.workflow.annotation.Polygon]
+- [`Polyline`][kolena.workflow.annotation.Polyline]
+- [`Keypoints`][kolena.workflow.annotation.Keypoints]
+- [`BoundingBox3D`][kolena.workflow.annotation.BoundingBox3D]
+- [`SegmentationMask`][kolena.workflow.annotation.SegmentationMask]
+- [`BitmapMask`][kolena.workflow.annotation.BitmapMask]
+- [`ClassificationLabel`][kolena.workflow.annotation.ClassificationLabel]
+
+For example, when viewing images in the Studio, any annotations (such as lists of
+[`BoundingBox`][kolena.workflow.annotation.BoundingBox] objects) present in the
+[`TestSample`][kolena.workflow.TestSample], [`GroundTruth`][kolena.workflow.GroundTruth],
+[`Inference`][kolena.workflow.Inference], or [`MetricsTestSample`][kolena.workflow.MetricsTestSample] objects are
+rendered on top of the image.
+"""
 from abc import ABCMeta
 from typing import Dict
 from typing import List
 from typing import Tuple
 
 from pydantic.dataclasses import dataclass
 
@@ -27,80 +47,83 @@
     BOUNDING_BOX = "BOUNDING_BOX"
     POLYGON = "POLYGON"
     POLYLINE = "POLYLINE"
     KEYPOINTS = "KEYPOINTS"
     BOUNDING_BOX_3D = "BOUNDING_BOX_3D"
     SEGMENTATION_MASK = "SEGMENTATION_MASK"
     BITMAP_MASK = "BITMAP_MASK"
-    CLASSIFICATON_LABEL = "LABEL"
+    CLASSIFICATION_LABEL = "LABEL"
 
     @staticmethod
     def _data_category() -> str:
         return "ANNOTATION"
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Annotation(TypedDataObject[_AnnotationType], metaclass=ABCMeta):
-    """
-    Where applicable, annotations are visualized in the web platform.
-
-    For example, when viewing images, any annotations present in a :class:`kolena.workflow.TestSample`,
-    :class:`kolena.workflow.GroundTruth`, :class:`kolena.workflow.Inference`, or
-    :class:`kolena.workflow.MetricsTestSample` are rendered on top of the image.
-    """
+    """The base class for all annotation types."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class BoundingBox(Annotation):
     """Rectangular bounding box specified with pixel coordinates of the top left and bottom right vertices."""
 
     top_left: Tuple[float, float]
+    """The top left vertex (in `(x, y)` image coordinates) of this bounding box."""
+
     bottom_right: Tuple[float, float]
+    """The bottom right vertex (in `(x, y)` image coordinates) of this bounding box."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.BOUNDING_BOX
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class LabeledBoundingBox(BoundingBox):
     """
     Rectangular bounding box specified with pixel coordinates of the top left and bottom right vertices and a string
     label.
     """
 
     label: str
+    """The label (e.g. model classification) associated with this bounding box."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ScoredBoundingBox(BoundingBox):
     """
     Rectangular bounding box specified with pixel coordinates of the top left and bottom right vertices and a float
     score.
     """
 
     score: float
+    """The score (e.g. model confidence) associated with this bounding box."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ScoredLabeledBoundingBox(BoundingBox):
     """
     Rectangular bounding box specified with pixel coordinates of the top left and bottom right vertices, a string
     label, and a float score.
     """
 
     label: str
+    """The label (e.g. model classification) associated with this bounding box."""
+
     score: float
+    """The score (e.g. model confidence) associated with this bounding box."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Polygon(Annotation):
     """Arbitrary polygon specified by three or more pixel coordinates."""
 
     points: List[Tuple[float, float]]
+    """The sequence of `(x, y)` points comprising the boundary of this polygon."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.POLYGON
 
     def __post_init__(self) -> None:
         if len(self.points) < 3:
@@ -108,154 +131,168 @@
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class LabeledPolygon(Polygon):
     """Arbitrary polygon specified by three or more pixel coordinates and a string label."""
 
     label: str
+    """The label (e.g. model classification) associated with this polygon."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ScoredPolygon(Polygon):
     """
     Arbitrary polygon specified by three or more pixel coordinates and a float score.
     """
 
     score: float
+    """The score (e.g. model confidence) associated with this polygon."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ScoredLabeledPolygon(Polygon):
     """
     Arbitrary polygon specified by three or more pixel coordinates with a string label and a float score.
     """
 
     label: str
+    """The label (e.g. model classification) associated with this polygon."""
+
     score: float
+    """The score (e.g. model confidence) associated with this polygon."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Keypoints(Annotation):
     """Array of any number of keypoints specified in pixel coordinates."""
 
     points: List[Tuple[float, float]]
+    """The sequence of discrete `(x, y)` points comprising this keypoints annotation."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.KEYPOINTS
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Polyline(Annotation):
     """Polyline with any number of vertices specified in pixel coordinates."""
 
     points: List[Tuple[float, float]]
+    """The sequence of connected `(x, y)` points comprising this polyline."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.POLYLINE
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class BoundingBox3D(Annotation):
     """
     Three-dimensional cuboid bounding box in a right-handed coordinate system.
 
-    Specified by (x, y, z) coordinates for the ``center`` of the cuboid, (x, y, z) ``dimensions``, and a ``rotation``
-    parameter specifying the degrees of rotation about each axis (x, y, z) ranging [-pi, pi].
+    Specified by `(x, y, z)` coordinates for the `center` of the cuboid, `(x, y, z)` `dimensions`, and a `rotation`
+    parameter specifying the degrees of rotation about each axis `(x, y, z)` ranging `[-π, π]`.
     """
 
-    #: (x, y, z) coordinates specifying the center of the bounding box.
     center: Tuple[float, float, float]
+    """`(x, y, z)` coordinates specifying the center of the bounding box."""
 
-    #: (x, y, z) measurements specifying the dimensions of the bounding box.
     dimensions: Tuple[float, float, float]
+    """`(x, y, z)` measurements specifying the dimensions of the bounding box."""
 
-    #: Rotations in degrees about each (x, y, z) axis.
     rotations: Tuple[float, float, float]
+    """Rotations in degrees about each `(x, y, z)` axis."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.BOUNDING_BOX_3D
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class LabeledBoundingBox3D(BoundingBox3D):
-    """:class:`BoundingBox3D` with an additional string label."""
+    """[`BoundingBox3D`][kolena.workflow.annotation.BoundingBox3D] with an additional string label."""
 
     label: str
+    """The label associated with this 3D bounding box."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ScoredBoundingBox3D(BoundingBox3D):
-    """:class:`BoundingBox3D` with an additional float score."""
+    """[`BoundingBox3D`][kolena.workflow.annotation.BoundingBox3D] with an additional float score."""
 
     score: float
+    """The score associated with this 3D bounding box."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ScoredLabeledBoundingBox3D(BoundingBox3D):
-    """:class:`BoundingBox3D` with an additional string label and float score."""
+    """[`BoundingBox3D`][kolena.workflow.annotation.BoundingBox3D] with an additional string label and float score."""
 
     label: str
+    """The label associated with this 3D bounding box."""
+
     score: float
+    """The score associated with this 3D bounding box."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class SegmentationMask(Annotation):
     """
-    Raster segmentation mask. The ``locator`` is the URL to the image file representing the segmentation mask.
+    Raster segmentation mask. The `locator` is the URL to the image file representing the segmentation mask.
 
     The segmentation mask must be rendered as a single-channel, 8-bit-depth (grayscale) image. For the best results,
     use a lossless file format such as PNG. Each pixel's value is the numerical ID of its class label, as specified in
-    the ``labels`` map. Any pixel value not present in the ``labels`` map is rendered as part of the background.
+    the `labels` map. Any pixel value not present in the `labels` map is rendered as part of the background.
 
-    For example, ``labels = {255: "object"}`` will highlight all pixels with the value of 255 as ``"object"``. Every
+    For example, `labels = {255: "object"}` will highlight all pixels with the value of 255 as `"object"`. Every
     other pixel value will be transparent.
     """
 
-    #: Mapping of unique label IDs (pixel values) to unique label values.
     labels: Dict[int, str]
+    """Mapping of unique label IDs (pixel values) to unique label values."""
 
-    #: URL of the image (segmentation mask).
     locator: str
+    """URL of the segmentation mask image."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.SEGMENTATION_MASK
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class BitmapMask(Annotation):
-    """Arbitrary bitmap mask. The ``locator`` is the URL to the image file representing the mask."""
+    """Arbitrary bitmap mask. The `locator` is the URL to the image file representing the mask."""
 
-    #: URL of the bitmap data.
     locator: str
+    """URL of the bitmap data."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.BITMAP_MASK
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ClassificationLabel(Annotation):
     """Label of classification."""
 
     label: str
+    """String label for this classification."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
-        return _AnnotationType.CLASSIFICATON_LABEL
+        return _AnnotationType.CLASSIFICATION_LABEL
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ScoredClassificationLabel(ClassificationLabel):
     """Classification label with accompanying score."""
 
     score: float
+    """Score associated with this label."""
 
 
 _ANNOTATION_TYPES = [
     BoundingBox,
     LabeledBoundingBox,
     ScoredBoundingBox,
     ScoredLabeledBoundingBox,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kolena_client-0.72.0/kolena/workflow/evaluator.py` & `kolena_client-0.73.0/kolena/workflow/evaluator.py`

 * *Files 22% similar despite different names*

```diff
@@ -42,79 +42,82 @@
 from kolena.workflow._validators import validate_data_object_type
 from kolena.workflow._validators import validate_scalar_data_object_type
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class MetricsTestSample(DataObject, metaclass=ABCMeta):
     """
-    Test-sample-level metrics produced by an :class:`Evaluator`.
+    Test-sample-level metrics produced by an [`Evaluator`][kolena.workflow.Evaluator].
 
     This class should be subclassed with the relevant fields for a given workflow.
 
     Examples here may include the number of true positive detections on an image, the mean IOU of inferred polygon(s)
     with ground truth polygon(s), etc.
     """
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         _validate_metrics_test_sample_type(cls)
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class MetricsTestCase(DataObject, metaclass=ABCMeta):
     """
-    Test-case-level metrics produced by an :class:`Evaluator`.
+    Test-case-level metrics produced by an [`Evaluator`][kolena.workflow.Evaluator].
 
     This class should be subclassed with the relevant fields for a given workflow.
 
     Test-case-level metrics are aggregate metrics like Precision, Recall, and F1 score. Any and all aggregate metrics
     that fit a workflow should be defined here.
 
-    ``MetricsTestCase`` supports nesting metrics objects, for e.g. reporting class-level metrics within a test case that
+    `MetricsTestCase` supports nesting metrics objects, for e.g. reporting class-level metrics within a test case that
     contains multiple classes. Example usage:
 
-    .. code-block:: python
-
-        @dataclass(frozen=True)
-        class PerClassMetrics(MetricsTestCase):
-            Class: str
-            Precision: float
-            Recall: float
-            F1: float
-            AP: float
-
-        @dataclass(frozen=True)
-        class TestCaseMetrics(MetricsTestCase):
-            macro_Precision: float
-            macro_Recall: float
-            macro_F1: float
-            mAP: float
-            PerClass: List[PerClassMetrics]
+    ```python
+    @dataclass(frozen=True)
+    class PerClassMetrics(MetricsTestCase):
+        Class: str
+        Precision: float
+        Recall: float
+        F1: float
+        AP: float
+
+    @dataclass(frozen=True)
+    class TestCaseMetrics(MetricsTestCase):
+        macro_Precision: float
+        macro_Recall: float
+        macro_F1: float
+        mAP: float
+        PerClass: List[PerClassMetrics]
+    ```
     """
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         _validate_metrics_test_case_type(cls)
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class MetricsTestSuite(DataObject, metaclass=ABCMeta):
     """
-    Test-suite-level metrics produced by an :class:`Evaluator`.
+    Test-suite-level metrics produced by an [`Evaluator`][kolena.workflow.Evaluator].
 
     This class should be subclassed with the relevant fields for a given workflow.
 
     Test-suite-level metrics typically measure performance across test cases, e.g. penalizing variance across different
     subsets of a benchmark.
     """
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         _validate_metrics_test_suite_type(cls)
 
 
 NumberSeries = Sequence[Union[float, int]]
+"""A sequence of numeric values."""
+
 NullableNumberSeries = Sequence[Union[float, int, None]]
+"""A sequence of numeric values or `None`."""
 
 
 class _PlotType(DataType):
     CURVE = "CURVE"
     CONFUSION_MATRIX = "CONFUSION_MATRIX"
     HISTOGRAM = "HISTOGRAM"
     BAR = "BAR"
@@ -122,35 +125,40 @@
     @staticmethod
     def _data_category() -> str:
         return "PLOT"
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class AxisConfig(DataObject):
-    """Configuration for the format of a given axis on a Plot"""
+    """Configuration for the format of a given axis on a plot."""
 
-    #: Type of axis to display. Supported options are `linear` and `log`.
     type: Literal["linear", "log"]
+    """Type of axis to display. Supported options are `linear` and `log`."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Plot(TypedDataObject[_PlotType], metaclass=ABCMeta):
     """A data visualization shown when exploring model results in the web platform."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Curve(DataObject):
-    """A single series on a :class:`CurvePlot`."""
+    """A single series on a [`CurvePlot`][kolena.workflow.CurvePlot]."""
 
     x: NumberSeries
+    """The `x` coordinates of this curve. Length must match the provided `y` coordinates."""
+
     y: NumberSeries
+    """The `y` coordinates of this curve. Length must match the provided `x` coordinates."""
 
-    #: Optionally specify an additional label (in addition to the associated test case) to apply to this curve, for use
-    #: when e.g. there are multiple curves generated per test case.
     label: Optional[str] = None
+    """
+    Optionally specify an additional label (in addition to the associated test case) to apply to this curve, for use
+    when e.g. there are multiple curves generated per test case.
+    """
 
     def __post_init_post_parse__(self) -> None:
         if len(self.x) != len(self.y):
             raise ValueError(
                 f"Series 'x' (length: {len(self.x)}) and 'y' (length: {len(self.y)}) have different lengths",
             )
 
@@ -161,61 +169,95 @@
     A plot visualizing one or more curves per test case.
 
     Examples include Receiver Operating Characteristic (ROC) curves, Precision versus Recall (PR) curves,
     Detection-Error Tradeoff (DET) curves, etc.
     """
 
     title: str
+    """The title for the plot."""
+
     x_label: str
+    """The label describing the plot's `x` axis."""
+
     y_label: str
+    """The label describing the plot's `y` axis."""
 
-    #: A test case may generate zero or more curves on a given plot. However, under most circumstances, a single curve
-    #: per test case is desirable.
     curves: List[Curve]
+    """
+    A test case may generate zero or more curves on a given plot. However, under most circumstances, a single curve
+    per test case is desirable.
+    """
 
-    #: Custom format options to allow for control over the display of the plot axes.
     x_config: Optional[AxisConfig] = None
+    """
+    Custom options to allow for control over the display of the plot `x` axis. See
+    [`AxisConfig`][kolena.workflow.AxisConfig] for details.
+    """
+
     y_config: Optional[AxisConfig] = None
+    """
+    Custom options to allow for control over the display of the plot `y` axis. See
+    [`AxisConfig`][kolena.workflow.AxisConfig] for details.
+    """
 
     @staticmethod
     def _data_type() -> _PlotType:
         return _PlotType.CURVE
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Histogram(Plot):
     """
     A plot visualizing distribution of one or more continuous values, e.g. distribution of an error metric across all
     samples within a test case.
 
-    For visualization of discrete values, see :class:`BarPlot`.
+    For visualization of discrete values, see [`BarPlot`][kolena.workflow.BarPlot].
     """
 
     title: str
+    """The title for the plot."""
+
     x_label: str
+    """The label describing the plot's `x` axis."""
+
     y_label: str
+    """The label describing the plot's `y` axis."""
 
-    #: A Histogram requires intervals to bucket the data. For ``n`` buckets, ``n+1`` consecutive bounds must be
-    #: specified in increasing order.
     buckets: NumberSeries
+    """
+    A Histogram requires intervals to bucket the data. For `n` buckets, `n+1` consecutive bounds must be specified in
+    increasing order.
+    """
 
-    #: For ``n`` buckets, there are ``n`` frequencies corresponding to the height of each bucket. The frequency at index
-    #: ``i`` corresponds to the bucket with bounds (``i``, ``i+1``) in ``buckets``.
-    #:
-    #: To specify multiple distributions for a given test case, multiple frequency series can be provided, corresponding
-    #: e.g. to the distribution for a given class within a test case, with name specified in ``labels``.
     frequency: Union[NumberSeries, Sequence[NumberSeries]]
+    """
+    For `n` buckets, there are `n` frequencies corresponding to the height of each bucket. The frequency at index `i`
+    corresponds to the bucket with bounds (`i`, `i+1`) in `buckets`.
+
+    To specify multiple distributions for a given test case, multiple frequency series can be provided, corresponding
+    e.g. to the distribution for a given class within a test case, with name specified in `labels`.
+
+    Specify a list of labels corresponding to the different `frequency` series when multiple series are provided.
+    Can be omitted when a single `frequency` series is provided.
+    """
 
-    #: Specify a list of labels corresponding to the different ``frequency`` series when multiple series are provided.
-    #: Can be omitted when a single ``frequency`` series is provided.
     labels: Optional[List[str]] = None
+    """Specify the label corresponding to a given distribution when multiple are specified in `frequency`."""
 
-    #: Custom format options to allow for control over the display of the plot axes.
     x_config: Optional[AxisConfig] = None
+    """
+    Custom options to allow for control over the display of the plot `x` axis. See
+    [`AxisConfig`][kolena.workflow.AxisConfig] for details.
+    """
+
     y_config: Optional[AxisConfig] = None
+    """
+    Custom options to allow for control over the display of the plot `y` axis. See
+    [`AxisConfig`][kolena.workflow.AxisConfig] for details.
+    """
 
     def __post_init_post_parse__(self) -> None:
         n_buckets = len(self.buckets)
         if n_buckets < 2:
             raise ValueError(f"Minimum 2 entries required in 'buckets' series (length: {n_buckets})")
         buckets_arr = np.array(self.buckets)
         if not np.all(buckets_arr[1:] > buckets_arr[:-1]):  # validate strictly increasing
@@ -237,29 +279,30 @@
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class BarPlot(Plot):
     """A plot visualizing a set of bars per test case."""
 
     title: str
+    """The plot title."""
 
-    #: Axis label for the axis along which the bars are laid out (``labels``).
     x_label: str
+    """Axis label for the axis along which the bars are laid out (`labels`)."""
 
-    #: Axis label for the axis corresponding to bar height (``values``).
     y_label: str
+    """Axis label for the axis corresponding to bar height (`values`)."""
 
-    #: Labels for each bar with corresponding height specified in ``values``.
     labels: Sequence[Union[str, int, float]]
+    """Labels for each bar with corresponding height specified in `values`."""
 
-    #: Values for each bar with corresponding label specified in ``labels``.
     values: NullableNumberSeries
+    """Values for each bar with corresponding label specified in `labels`."""
 
-    #: Custom format options to allow for control over the display of the numerical plot axis (``values``).
     config: Optional[AxisConfig] = None
+    """Custom format options to allow for control over the display of the numerical plot axis (`values`)."""
 
     def __post_init_post_parse__(self) -> None:
         n_labels, n_values = len(self.labels), len(self.values)
         if n_labels == 0 or n_values == 0 or n_labels != n_values:
             raise ValueError(
                 f"Series 'labels' (length: {n_labels}) and 'values' (length: {n_values}) "
                 "must be equal length and non-empty",
@@ -271,41 +314,50 @@
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ConfusionMatrix(Plot):
     """
     A confusion matrix. Example:
 
-    .. code-block:: python
-
-        ConfusionMatrix(
-            title="Cat and Dog Confusion",
-            labels=["Cat", "Dog"],
-            matrix=[[90, 10], [5, 95]],
-        )
+    ```python
+    ConfusionMatrix(
+        title="Cat and Dog Confusion",
+        labels=["Cat", "Dog"],
+        matrix=[[90, 10], [5, 95]],
+    )
+    ```
 
     Yields a confusion matrix of the form:
 
-    .. code-block:: none
+    ```
+                Predicted
 
-                    Predicted
-
-                    Cat   Dog
-                   +----+----+
-               Cat | 90 | 10 |
-        Actual     +----+----+
-               Dog |  5 | 95 |
-                   +----+----+
+                Cat   Dog
+               +----+----+
+           Cat | 90 | 10 |
+    Actual     +----+----+
+           Dog |  5 | 95 |
+               +----+----+
+    ```
     """
 
     title: str
+    """The plot title."""
+
     labels: List[str]
+    """The labels corresponding to each entry in the square `matrix`."""
+
     matrix: Sequence[NullableNumberSeries]
+    """A square matrix, typically representing the number of matches between class `i` and class `j`."""
+
     x_label: str = "Predicted"
+    """The label for the `x` axis of the confusion matrix."""
+
     y_label: str = "Actual"
+    """The label for the `y` axis of the confusion matrix."""
 
     def __post_init_post_parse__(self) -> None:
         n_labels = len(self.labels)
         if n_labels < 2:
             raise ValueError(f"At least two labels required: got {n_labels}")
         if len(self.matrix) != n_labels:
             raise ValueError(f"Invalid number of matrix rows: got {len(self.matrix)}, expected {n_labels}")
@@ -317,127 +369,143 @@
     def _data_type() -> _PlotType:
         return _PlotType.CONFUSION_MATRIX
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class EvaluatorConfiguration(DataObject, metaclass=ABCMeta):
     """
-    Configuration for an :class:`Evaluator`.
+    Configuration for an [`Evaluator`][kolena.workflow.Evaluator].
 
     Example evaluator configurations may specify:
 
     - Fixed confidence thresholds at which detections are discarded.
     - Different algorithms/strategies used to compute confidence thresholds
         (e.g. "accuracy optimal" for a classification-type workflow).
     """
 
     @abstractmethod
     def display_name(self) -> str:
+        """
+        The name to display for this configuration in Kolena. Must be implemented when extending
+        [`EvaluatorConfiguration`][kolena.workflow.EvaluatorConfiguration].
+        """
         raise NotImplementedError
 
 
 class Evaluator(metaclass=ABCMeta):
     """
-    An :class:`kolena.workflow.Evaluator` transforms inferences into metrics.
+    An `Evaluator` transforms inferences into metrics.
 
-    Metrics are computed at the individual test sample level (:class:`kolena.workflow.MetricsTestSample`), in aggregate
-    at the test case level (:class:`kolena.workflow.MetricsTestCase`), and across populations at the test suite level
-    (:class:`kolena.workflow.MetricsTestSuite`).
+    Metrics are computed at the individual test sample level ([`MetricsTestSample`][kolena.workflow.MetricsTestSample]),
+    in aggregate at the test case level ([`MetricsTestCase`][kolena.workflow.MetricsTestCase]), and across populations
+    at the test suite level ([`MetricsTestSuite`][kolena.workflow.MetricsTestSuite]).
 
-    Test-case-level plots (:class:`kolena.workflow.Plot`) may also be computed.
+    Test-case-level plots ([`Plot`][kolena.workflow.Plot]) may also be computed.
+
+    :param configurations: The configurations at which to perform evaluation. Instance methods such as
+        [`compute_test_sample_metrics`][kolena.workflow.Evaluator.compute_test_sample_metrics] are called once per test
+        case per configuration.
     """
 
     configurations: List[EvaluatorConfiguration]
+    """The configurations with which to perform evaluation, provided on instantiation."""
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, configurations: Optional[List[EvaluatorConfiguration]] = None):
         if configurations is not None and len(configurations) == 0:
             raise ValueError("empty configuration list provided, at least one configuration required or 'None'")
         self.configurations = configurations or []
         if len({configuration.display_name() for configuration in self.configurations}) < len(self.configurations):
             raise ValueError("all configurations must have distinct display names")
 
     def display_name(self) -> str:
+        """The name to display for this evaluator in Kolena. Defaults to the name of this class."""
         return type(self).__name__
 
     @abstractmethod
     def compute_test_sample_metrics(
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         configuration: Optional[EvaluatorConfiguration] = None,
     ) -> List[Tuple[TestSample, MetricsTestSample]]:
         """
-        Compute metrics for every test sample in a test case.
+        Compute metrics for every test sample in a test case, i.e. one
+        [`MetricsTestSample`][kolena.workflow.MetricsTestSample] object for each of the provided test samples.
 
         Must be implemented.
 
-        :param test_case: the test case to which the provided test samples and ground truths belong.
-        :param inferences: the test samples, ground truths, and inferences for all entries in a test case.
-        :param configuration: the evaluator configuration to use. Empty for implementations that are not configured.
-        :return: test-sample-level metrics for each provided test sample.
+        :param test_case: The [`TestCase`][kolena.workflow.TestCase] to which the provided test samples and ground
+            truths belong.
+        :param inferences: The test samples, ground truths, and inferences for all entries in a test case.
+        :param configuration: The evaluator configuration to use. Empty for implementations that are not configured.
+        :return: [`TestSample`][kolena.workflow.TestSample]-level metrics for each provided test sample.
         """
         raise NotImplementedError
 
     @abstractmethod
     def compute_test_case_metrics(
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[MetricsTestSample],
         configuration: Optional[EvaluatorConfiguration] = None,
     ) -> MetricsTestCase:
         """
-        Compute aggregate metrics across a test case.
+        Compute aggregate metrics ([`MetricsTestCase`][kolena.workflow.MetricsTestCase]) across a test case.
 
         Must be implemented.
 
-        :param test_case: the test case in question.
-        :param inferences: the test samples, ground truths, and inferences for all entries in a test case.
-        :param metrics: the test-sample-level metrics computed by :meth:`Evaluator.compute_test_sample_metrics`.
-            Provided in the same order as ``inferences``.
-        :param configuration: the evaluator configuration to use. Empty for implementations that are not configured.
-        :return: test-case-level metrics for the provided test case.
+        :param test_case: The test case in question.
+        :param inferences: The test samples, ground truths, and inferences for all entries in a test case.
+        :param metrics: The [`TestSample`][kolena.workflow.TestSample]-level metrics computed by
+            [`compute_test_sample_metrics`][kolena.workflow.Evaluator.compute_test_sample_metrics], provided
+            in the same order as `inferences`.
+        :param configuration: The evaluator configuration to use. Empty for implementations that are not configured.
+        :return: [`TestCase`][kolena.workflow.TestCase]-level metrics for the provided test case.
         """
         raise NotImplementedError
 
     @validate_arguments(config=ValidatorConfig)
     def compute_test_case_plots(
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[MetricsTestSample],
         configuration: Optional[EvaluatorConfiguration] = None,
     ) -> Optional[List[Plot]]:
         """
         Optionally compute any number of plots to visualize the results for a test case.
 
-        :param test_case: the test case in question
-        :param inferences: the test samples, ground truths, and inferences for all entries in a test case.
-        :param metrics: the test-sample-level metrics computed by :meth:`Evaluator.compute_test_sample_metrics`.
-            Provided in the same order as ``inferences``.
+        :param test_case: The test case in question
+        :param inferences: The test samples, ground truths, and inferences for all entries in a test case.
+        :param metrics: The [`TestSample`][kolena.workflow.TestSample]-level metrics computed by
+            [`compute_test_sample_metrics`][kolena.workflow.Evaluator.compute_test_sample_metrics], provided
+            in the same order as `inferences`.
         :param configuration: the evaluator configuration to use. Empty for implementations that are not configured.
-        :return: zero or more plots for this test case at this configuration.
+        :return: Zero or more plots for this test case at this configuration.
         """
         return None  # not required
 
     @validate_arguments(config=ValidatorConfig)
     def compute_test_suite_metrics(
         self,
         test_suite: TestSuite,
         metrics: List[Tuple[TestCase, MetricsTestCase]],
         configuration: Optional[EvaluatorConfiguration] = None,
     ) -> Optional[MetricsTestSuite]:
         """
-        Optionally compute test-suite-level metrics.
+        Optionally compute [`TestSuite`][kolena.workflow.TestSuite]-level metrics
+        ([`MetricsTestSuite`][kolena.workflow.MetricsTestSuite]) across the provided `test_suite`.
 
-        :param test_suite: the test suite in question
-        :param metrics: the test-case-level metrics computed by :meth:`Evaluator.compute_test_case_metrics`
-        :param configuration: the evaluator configuration to use. Empty for implementations that are not configured.
-        :return: the test-suite-level metrics for this test suite
+        :param test_suite: The test suite in question.
+        :param metrics: The [`TestCase`][kolena.workflow.TestCase]-level metrics computed by
+            [`compute_test_case_metrics`][kolena.workflow.Evaluator.compute_test_case_metrics].
+        :param configuration: The evaluator configuration to use. Empty for implementations that are not configured.
+        :return: The [`TestSuite`][kolena.workflow.TestSuite]-level metrics for this test suite.
         """
         return None  # not required
 
 
 def _validate_metrics_test_sample_type(metrics_test_sample_type: Type[MetricsTestSample]) -> None:
     # TODO: support special structure for ImagePair test sample types?
     validate_data_object_type(metrics_test_sample_type)
```

### Comparing `kolena_client-0.72.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.73.0/kolena/workflow/evaluator_function.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+Simplified interface for [`Evaluator`][kolena.workflow.Evaluator] implementations.
+"""
 import dataclasses
 import json
 from abc import ABCMeta
 from abc import abstractmethod
 from dataclasses import field
 from inspect import signature
 from typing import Callable
@@ -61,100 +64,116 @@
         ground_truths: List[GroundTruth],
         inferences: List[Inference],
         metrics_test_sample: List[MetricsTestSample],
     ) -> Iterator[Tuple[TestCase, List[TestSample], List[GroundTruth], List[Inference], List[MetricsTestSample]]]:
         """
         Matches test sample metrics to the corresponding test cases that they belong to.
 
-        :param test_samples: all unique test samples within the test run, sequenced in the same order as the other
+        :param test_samples: All unique test samples within the test run, sequenced in the same order as the other
             parameters.
-        :param ground_truths: ground truths corresponding to ``test_samples``, sequenced in the same order.
-        :param inferences: inferences corresponding to ``test_samples``, sequenced in the same order.
-        :param metrics_test_sample: test-sample-level metrics corresponding to ``test_samples``, sequenced in the
+        :param ground_truths: Ground truths corresponding to `test_samples`, sequenced in the same order.
+        :param inferences: Inferences corresponding to `test_samples`, sequenced in the same order.
+        :param metrics_test_sample: Test-sample-level metrics corresponding to `test_samples`, sequenced in the
             same order.
-        :return: an iterator that groups each test case in the test run to the lists of member test samples, inferences,
+        :return: Iterator that groups each test case in the test run to the lists of member test samples, inferences,
             and test-sample-level metrics.
         """
         raise NotImplementedError
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class EvaluationResults:
     """
     A bundle of metrics computed for a test run grouped at the test-sample-level, test-case-level, and test-suite-level.
-    Optionally includes :class:`kolena.workflow.Plot`s at the test-case-level.
+    Optionally includes [`Plot`s][kolena.workflow.Plot] at the test-case-level.
     """
 
     metrics_test_sample: List[Tuple[BaseTestSample, BaseMetricsTestSample]]
+    """
+    Sample-level metrics, extending [`MetricsTestSample`][kolena.workflow.MetricsTestSample], for every provided test
+    sample.
+    """
+
     metrics_test_case: List[Tuple[TestCase, MetricsTestCase]]
+    """
+    Aggregate metrics, extending [`MetricsTestCase`][kolena.workflow.MetricsTestCase], computed across each test case
+    yielded from [`TestCases.iter`][kolena.workflow.TestCases.iter].
+    """
+
     plots_test_case: List[Tuple[TestCase, List[Plot]]] = field(default_factory=list)
+    """Optional test-case-level plots."""
+
     metrics_test_suite: Optional[MetricsTestSuite] = None
+    """Optional test-suite-level metrics, extending [`MetricsTestSuite`][kolena.workflow.MetricsTestSuite]."""
 
 
 ConfiguredEvaluatorFunction = Callable[
     [List[TestSample], List[GroundTruth], List[Inference], TestCases, EvaluatorConfiguration],
     Optional[EvaluationResults],
 ]
 UnconfiguredEvaluatorFunction = Callable[
     [List[TestSample], List[GroundTruth], List[Inference], TestCases],
     Optional[EvaluationResults],
 ]
-#: ``kolena.workflow.BasicEvaluatorFunction`` introduces a function based evaluator implementation that takes
-#: the inferences for all test samples in a test suite and a :class:`kolena.workflow.TestCases` as input, and computes
-#: the corresponding test-sample-level, test-case-level, and test-suite-level metrics (and optionally plots) as output.
-#:
-#: Example implementation, relying on ``compute_per_sample`` and ``compute_aggregate`` functions implemented elsewhere:
-#:
-#: .. code-block:: python
-#:
-#:     def evaluate(
-#:         test_samples: List[TestSample],
-#:         ground_truths: List[GroundTruth],
-#:         inferences: List[Inference],
-#:         test_cases: TestCases,
-#:     ) -> EvaluationResults:
-#:         # compute per-sample metrics for each test sample
-#:         per_sample_metrics = [compute_per_sample(gt, inf) for gt, inf in zip(ground_truths, inferences)]
-#:
-#:         # compute aggregate metrics across all test cases using `test_cases.iter(...)`
-#:         aggregate_metrics: List[Tuple[TestCase, MetricsTestCase]] = []
-#:         for test_case, *s in test_cases.iter(test_samples, ground_truths, inferences, per_sample_metrics):
-#:             # subset of `test_samples`/`ground_truths`/`inferences`/`test_sample_metrics` in given test case
-#:             tc_test_samples, tc_ground_truths, tc_inferences, tc_per_sample_metrics = s
-#:             aggregate_metrics.append((test_case, compute_aggregate(tc_per_sample_metrics)))
-#:
-#:         # if desired, compute and add `plots_test_case` and `metrics_test_suite`
-#:         return EvaluationResults(
-#:             metrics_test_sample=list(zip(test_samples, per_sample_metrics)),
-#:             metrics_test_case=aggregate_metrics,
-#:         )
-#:
-#: The control flow is in general more streamlined than with :class:`kolena.workflow.Evaluator`, but requires a couple
-#: of assumptions to hold:
-#:
-#: - Test-sample-level metrics do not vary by test case
-#: - Ground truths corresponding to a given test sample do not vary by test case
-#:
-#: This ``BasicEvaluatorFunction`` is provided to the test run at runtime, and is expected to have the
-#: following signature:
-#:
-#: :param List[kolena.workflow.TestSample] test_samples: A list of distinct :class:`kolena.workflow.TestSample` values
-#:     that correspond to all test samples in the test run.
-#: :param List[kolena.workflow.GroundTruth] ground_truths: A list of :class:`kolena.workflow.GroundTruth` values
-#:     corresponding to and sequenced in the same order as ``test_samples``.
-#: :param List[kolena.workflow.Inference] inferences: A list of :class:`kolena.workflow.Inference` values corresponding
-#:     to and sequenced in the same order as ``test_samples``.
-#: :param TestCases test_cases: An instance of :class:`kolena.workflow.TestCases`, generally used to provide iteration
-#:        groupings for evaluating test-case-level metrics.
-#: :param EvaluatorConfiguration evaluator_configuration: The configuration to use when performing the evaluation.
-#:     This parameter may be omitted in the function definition if running with no configuration.
-#: :rtype: :class:`kolena.workflow.EvaluationResults`
-#: :return: An object tracking the test-sample-level, test-case-level and test-suite-level metrics and plots for the
-#:     input collection of test samples.
 BasicEvaluatorFunction = Union[ConfiguredEvaluatorFunction, UnconfiguredEvaluatorFunction]
+"""
+`BasicEvaluatorFunction` provides a function-based evaluator interface that takes
+the inferences for all test samples in a test suite and a [`TestCases`][kolena.workflow.TestCases] as input and computes
+the corresponding test-sample-level, test-case-level, and test-suite-level metrics (and optionally plots) as output.
+
+Example implementation, relying on `compute_per_sample` and `compute_aggregate` functions implemented elsewhere:
+
+```python
+def evaluate(
+    test_samples: List[TestSample],
+    ground_truths: List[GroundTruth],
+    inferences: List[Inference],
+    test_cases: TestCases,
+    # configuration: EvaluatorConfiguration,  # uncomment when configuration is used
+) -> EvaluationResults:
+    # compute per-sample metrics for each test sample
+    per_sample_metrics = [compute_per_sample(gt, inf) for gt, inf in zip(ground_truths, inferences)]
+
+    # compute aggregate metrics across all test cases using `test_cases.iter(...)`
+    aggregate_metrics: List[Tuple[TestCase, MetricsTestCase]] = []
+    for test_case, *s in test_cases.iter(test_samples, ground_truths, inferences, per_sample_metrics):
+        # subset of `test_samples`/`ground_truths`/`inferences`/`test_sample_metrics` in given test case
+        tc_test_samples, tc_ground_truths, tc_inferences, tc_per_sample_metrics = s
+        aggregate_metrics.append((test_case, compute_aggregate(tc_per_sample_metrics)))
+
+    # if desired, compute and add `plots_test_case` and `metrics_test_suite`
+    return EvaluationResults(
+        metrics_test_sample=list(zip(test_samples, per_sample_metrics)),
+        metrics_test_case=aggregate_metrics,
+    )
+```
+
+The control flow is in general more streamlined than with [`Evaluator`][kolena.workflow.Evaluator], but requires a
+couple of assumptions to hold:
+
+- Test-sample-level metrics do not vary by test case
+- Ground truths corresponding to a given test sample do not vary by test case
+
+This `BasicEvaluatorFunction` is provided to the test run at runtime, and is expected to have the following signature:
+
+:param List[TestSample] test_samples: A list of distinct [`TestSample`][kolena.workflow.TestSample] values
+    that correspond to all test samples in the test run.
+:param List[GroundTruth] ground_truths: A list of [`GroundTruth`][kolena.workflow.GroundTruth] values
+    corresponding to and sequenced in the same order as `test_samples`.
+:param List[Inference] inferences: A list of [`Inference`][kolena.workflow.Inference] values corresponding
+    to and sequenced in the same order as `test_samples`.
+:param TestCases test_cases: An instance of [`TestCases`][kolena.workflow.TestCases], used to provide iteration
+    groupings for evaluating test-case-level metrics.
+:param EvaluatorConfiguration evaluator_configuration: The
+    [`EvaluatorConfiguration`][kolena.workflow.EvaluatorConfiguration] to use when performing the evaluation. This
+    parameter may be omitted in the function definition for implementations that do not use any configuration object.
+:rtype: EvaluationResults
+:return: An [`EvaluationResults`][kolena.workflow.EvaluationResults] object tracking the test-sample-level,
+    test-case-level and test-suite-level metrics and plots for the input collection of test samples.
+"""
 
 
 class _TestCases(TestCases):
     def __init__(
         self,
         test_case_membership: List[Tuple[TestCase, List[TestSample]]],
         test_run_id: int,
@@ -193,15 +212,15 @@
     def _update_progress(self, test_case: TestCase) -> None:
         if not is_client_initialized():
             return
 
         config_description = (
             f" {_configuration_description(self._wip_configuration)}" if self._wip_configuration else ""
         )
-        message = f"Computed metrics for test case '{test_case.name}' (v{test_case.version}){config_description}"
+        message = f"computed metrics for test case '{test_case.name}' (v{test_case.version}){config_description}"
         progress = self._n_test_cases_processed / self._n_test_cases_and_configurations
 
         log.info(message)
         request = API.UpdateMetricsStatusRequest(
             test_run_id=self._test_run_id,
             progress=progress,
             message=message,
```

### Comparing `kolena_client-0.72.0/kolena/workflow/ground_truth.py` & `kolena_client-0.73.0/kolena/workflow/ground_truth.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,35 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+The ground truth associated with a [`TestSample`][kolena.workflow.TestSample]. Typically, a ground truth will represent
+the expected output of a model when given a test sample and will be manually annotated by a human.
+
+```python
+from dataclasses import dataclass
+from typing import List
+
+from kolena.workflow import GroundTruth
+from kolena.workflow.annotation import Polyline, SegmentationMask
+
+@dataclass(frozen=True)
+class AvGroundTruth(GroundTruth):
+    road_area: SegmentationMask
+    lane_boundaries: List[Polyline]
+    visibility_score: int
+```
+
+A [`TestCase`][kolena.workflow.TestCase] holds a list of test samples (model inputs) paired with ground truths
+(expected outputs).
+"""
 from typing import Type
 
 from pydantic.dataclasses import dataclass
 
 from kolena._utils.validators import ValidatorConfig
 from kolena.workflow import Composite
 from kolena.workflow import TestSample
@@ -27,46 +48,49 @@
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class GroundTruth(DataObject):
     """
     The ground truth against which a model is evaluated.
 
-    A test case contains one or more :class:`kolena.workflow.TestSample` objects each paired with a ground truth object.
-    During evaluation, these test samples, ground truths, and your model's inferences are provided to the
-    :class:`kolena.workflow.Evaluator` implementation.
+    A test case contains one or more [`TestSample`][kolena.workflow.TestSample] objects each paired with a ground truth
+    object. During evaluation, these test samples, ground truths, and your model's inferences are provided to the
+    [`Evaluator`][kolena.workflow.Evaluator] implementation.
+
+    This object may contain any combination of scalars (e.g. `str`, `float`),
+    [`Annotation`][kolena.workflow.annotation.Annotation] objects, or lists of these objects.
+
+    For [`Composite`][kolena.workflow.Composite], each object can contain multiple basic test sample elements. To
+    associate a set of attributes and/or annotations as the ground truth to a target test sample element, declare
+    annotations by extending `DataObject` and use the same attribute name as used in the
+    [`Composite`][kolena.workflow.Composite] test sample.
+
+    Continue with the example given in [`Composite`][kolena.workflow.Composite], where the `FacePairSample` test sample
+    type is defined using a pair of images under the `source` and `target` members, we can design a corresponding ground
+    truth type with image-level annotations defined in the `FaceRegion` object:
+
+    ```python
+    from dataclasses import dataclass
+
+    from kolena.workflow import DataObject, GroundTruth
+    from kolena.workflow.annotation import BoundingBox, Keypoints
+
+    @dataclass(frozen=True)
+    class FaceRegion(DataObject):
+        bounding_box: BoundingBox
+        keypoints: Keypoints
+
+    @dataclass(frozen=True)
+    class FacePair(GroundTruth):
+        source: FaceRegion
+        target: FaceRegion
+        is_same_person: bool
+    ```
 
-    This object may contain any combination of scalars (e.g. ``str``, ``float``),
-    :class:`kolena.workflow.annotation.Annotation` objects, or lists of these objects.
-
-    For :class:`kolena.workflow.Composite`, each object can contain multiple basic test sample elements.
-    To associate a set of attributes and/or annotations as the ground truth to a target test sample element,
-    one can use :class:`kolena.workflow.DataObject` and use the same name as in :class:`kolena.workflow.Composite`.
-
-    Continue with the example given in :class:`kolena.workflow.Composite`, which takes an image pair as a
-    test sample, one can design ground truth as:
-
-    .. code-block:: python
-
-        class FacePairSample(kolena.workflow.Composite):
-            source: Image
-            target: Image
-
-
-        class FaceRegion(DataObject):
-            bounding_box: BoundingBox
-            keypoints: Keypoints
-
-
-        class FacePair(GroundTruth):
-            source: FaceRegion
-            target: FaceRegion
-            is_same_person: bool
-
-    making it clear which bounding boxes and keypoints are associated to which image in the test sample.
+    This way, it is clear which bounding boxes and keypoints are associated to which image in the test sample.
     """
 
 
 def _validate_ground_truth_type(
     test_sample_type: Type[TestSample],
     ground_truth_type: Type[GroundTruth],
 ) -> None:
```

### Comparing `kolena_client-0.72.0/kolena/workflow/inference.py` & `kolena_client-0.73.0/kolena/workflow/inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,31 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+The output from a [`Model`][kolena.workflow.Model]. In other words, a model is a deterministic transformation from a
+[`TestSample`][kolena.workflow.TestSample] to an [`Inference`][kolena.workflow.Inference].
+
+```python
+from dataclasses import dataclass
+from typing import Optional
+
+from kolena.workflow import Inference
+from kolena.workflow.annotation import Keypoints
+
+@dataclass(frozen=True)
+class PoseEstimate(Inference):
+    skeleton: Optional[Keypoints] = None  # leave empty if nothing is detected
+    confidence: Optional[float] = None
+```
+"""
 from typing import Type
 
 from pydantic.dataclasses import dataclass
 
 from kolena._utils.validators import ValidatorConfig
 from kolena.workflow import Composite
 from kolena.workflow import TestSample
@@ -27,46 +44,49 @@
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Inference(DataObject):
     """
     The inference produced by a model.
 
-    Typically the structure of this object closely mirrors the structure of the :class:`kolena.workflow.GroundTruth` for
-    a workflow, but this is not a requirement.
+    Typically the structure of this object closely mirrors the structure of the
+    [`GroundTruth`][kolena.workflow.GroundTruth] for a workflow, but this is not a requirement.
 
-    During evaluation, the :class:`kolena.workflow.TestSample` objects, ground truth objects, and these inference
-    objects are provided to the :class:`kolena.workflow.Evaluator` implementation to compute metrics.
+    During evaluation, the [`TestSample`][kolena.workflow.TestSample] objects, ground truth objects, and these inference
+    objects are provided to the [`Evaluator`][kolena.workflow.Evaluator] implementation to compute metrics.
 
-    This object may contain any combination of scalars (e.g. ``str``, ``float``),
-    :class:`kolena.workflow.annotation.Annotation` objects, or lists of these objects.
+    This object may contain any combination of scalars (e.g. `str`, `float`),
+    [`Annotation`][kolena.workflow.annotation.Annotation] objects, or lists of these objects.
 
-    A model processing a :class:`kolean.workflow.Composite` object can produce an inference result for each of its
-    element. To associate an inference result to each test sample element, one can put the attributes and/or annotations
-    inside an :class:`kolena.workflow.DataObject` and use the same name as that in :class:`kolena.workflow.Composite`.
-
-    Continue with the example given in :class:`kolena.workflow.Composite`, which takes an image pair as a
-    test sample, one can design inference as:
-
-    .. code-block:: python
-
-        class FacePairSample(kolena.workflow.Composite):
-            source: Image
-            target: Image
-
-
-        class FaceRegion(DataObject):
-            bounding_box: BoundingBox
-            keypoints: Keypoints
-
-
-        class FacePair(Inference):
-            source: FaceRegion
-            target: FaceRegion
-            similarity: float
+    A model processing a [`Composite`][kolena.workflow.Composite] test sample can produce an inference result for each
+    of its elements. To associate an inference result to each test sample element, put the attributes and/or annotations
+    inside a `DataObject` and use the same attribute name as that used in the [`Composite`][kolena.workflow.Composite]
+    test sample.
+
+    Continue with the example given in [`Composite`][kolena.workflow.Composite], where the `FacePairSample` test sample
+    type is defined using a pair of images under the `source` and `target` members, we can design a corresponding
+    inference type with image-level annotations defined in the `FaceRegion` object:
+
+    ```python
+    from dataclasses import dataclass
+
+    from kolena.workflow import DataObject, Inference
+    from kolena.workflow.annotation import BoundingBox, Keypoints
+
+    @dataclass(frozen=True)
+    class FaceRegion(DataObject):
+        bounding_box: BoundingBox
+        keypoints: Keypoints
+
+    @dataclass(frozen=True)
+    class FacePair(Inference):
+        source: FaceRegion
+        target: FaceRegion
+        similarity: float
+    ```
 
     This way, it is clear which bounding boxes and keypoints are associated to which image in the test sample.
     """
 
 
 def _validate_inference_type(test_sample_type: Type[TestSample], inference_type: Type[Inference]) -> None:
     if not issubclass(inference_type, Inference):
```

### Comparing `kolena_client-0.72.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.73.0/kolena/workflow/metrics/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from ._geometry import InferenceMatches
 from ._geometry import iou
 from ._geometry import match_inferences
 from ._geometry import match_inferences_multiclass
+from ._geometry import MulticlassInferenceMatches
 
 __all__ = [
-    "InferenceMatches",
     "iou",
+    "InferenceMatches",
     "match_inferences",
+    "MulticlassInferenceMatches",
     "match_inferences_multiclass",
+    "MulticlassInferenceMatches",
 ]
```

### Comparing `kolena_client-0.72.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.73.0/kolena/workflow/metrics/_geometry.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict
-from dataclasses import dataclass
 from typing import Dict
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
 
-from shapely.geometry import Polygon as ShapelyPolygon
-from shapely.validation import make_valid
-
-from kolena.errors import InputValidationError
-
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
+from shapely.geometry import Polygon as ShapelyPolygon
+from shapely.validation import make_valid
+from pydantic.dataclasses import dataclass
+
+from kolena.errors import InputValidationError
 from kolena.workflow.annotation import BoundingBox
 from kolena.workflow.annotation import LabeledBoundingBox
 from kolena.workflow.annotation import LabeledPolygon
 from kolena.workflow.annotation import Polygon
 from kolena.workflow.annotation import ScoredBoundingBox
 from kolena.workflow.annotation import ScoredLabeledBoundingBox
 from kolena.workflow.annotation import ScoredLabeledPolygon
@@ -71,17 +70,17 @@
     return iou
 
 
 def iou(a: Union[BoundingBox, Polygon], b: Union[BoundingBox, Polygon]) -> float:
     """
     Compute the Intersection Over Union (IOU) of two geometries.
 
-    :param a: the first geometry in computation.
-    :param b: the second geometry in computation.
-    :return: the value of the IOU between geometries ``a`` and ``b``.
+    :param a: The first geometry in computation.
+    :param b: The second geometry in computation.
+    :return: The value of the IOU between geometries `a` and `b`.
     """
 
     if isinstance(a, BoundingBox) and isinstance(b, BoundingBox):
         return _iou_bbox(a, b)
 
     def as_shapely_polygon(obj: Union[BoundingBox, Polygon]) -> ShapelyPolygon:
         if isinstance(obj, BoundingBox):
@@ -98,31 +97,35 @@
 GT = TypeVar("GT", bound=Union[BoundingBox, Polygon])
 Inf = TypeVar("Inf", bound=Union[ScoredBoundingBox, ScoredPolygon, ScoredLabeledBoundingBox, ScoredLabeledPolygon])
 
 
 @dataclass(frozen=True)
 class InferenceMatches(Generic[GT, Inf]):
     """
-    The result of :func:`match_inferences`, providing lists of matches between ground truth and inference objects,
-    unmatched ground truths, and unmatched inferences. After applying some confidence threshold on returned inference
-    objects, :class:`InferenceMatches` can be used to calculate metrics such as precision and recall.
-
-    Objects are of type :class:`BoundingBox` or :class:`Polygon`, depending on the type of inputs provided to
-    :func:`match_inferences`.
+    The result of [`match_inferences`][kolena.workflow.metrics.match_inferences], providing lists of matches between
+    ground truth and inference objects, unmatched ground truths, and unmatched inferences. After applying some
+    confidence threshold on returned inference objects, `InferenceMatches` can be used to calculate metrics such as
+    precision and recall.
+
+    Objects are of type [`BoundingBox`][kolena.workflow.annotation.BoundingBox] or
+    [`Polygon`][kolena.workflow.annotation.Polygon], depending on the type of inputs provided to
+    [`match_inferences`][kolena.workflow.metrics.match_inferences].
     """
 
-    #: Pairs of matched ground truth and inference objects above the IOU threshold. Considered as true positive
-    #: detections after applying some confidence threshold.
     matched: List[Tuple[GT, Inf]]
+    """
+    Pairs of matched ground truth and inference objects above the IOU threshold. Considered as true positive
+    detections after applying some confidence threshold.
+    """
 
-    #: Unmatched ground truth objects. Considered as false negatives.
     unmatched_gt: List[GT]
+    """Unmatched ground truth objects. Considered as false negatives."""
 
-    #: Unmatched inference objects. Considered as false positives after applying some confidence threshold.
     unmatched_inf: List[Inf]
+    """Unmatched inference objects. Considered as false positives after applying some confidence threshold."""
 
 
 def _match_inferences_single_class_pascal_voc(
     ground_truths: List[GT],
     inferences: List[Inf],
     ignored_ground_truths: Optional[List[GT]] = None,
     iou_threshold: float = 0.5,
@@ -169,31 +172,37 @@
     mode: Literal["pascal"] = "pascal",
     iou_threshold: float = 0.5,
 ) -> InferenceMatches[GT, Inf]:
     """
     Matches model inferences with annotated ground truths using the provided configuration.
 
     This matcher does not consider labels, which is appropriate for single class object matching. To match with multiple
-    classes (i.e. heeding ``label`` classifications), use the multiclass matcher :func:`match_inferences_multiclass`.
+    classes (i.e. heeding `label` classifications), use the multiclass matcher
+    [`match_inferences_multiclass`][kolena.workflow.metrics.match_inferences_multiclass].
 
     Available modes:
 
-    - ``pascal`` (PASCAL VOC): For every inference by order of highest confidence, the ground truth of highest IOU is
+    - `pascal` (PASCAL VOC): For every inference by order of highest confidence, the ground truth of highest IOU is
       its match. Multiple inferences are able to match with the same ignored ground truth. See the
-      `PASCAL VOC paper <https://homepages.inf.ed.ac.uk/ckiw/postscript/ijcv_voc09.pdf>`_ for more information.
+      [PASCAL VOC paper](https://homepages.inf.ed.ac.uk/ckiw/postscript/ijcv_voc09.pdf) for more information.
 
-    :param List[Geometry] ground_truths: a list of :class:`BoundingBox` or :class:`Polygon` ground truths.
-    :param List[ScoredGeometry] inferences: a list of :class:`ScoredBoundingBox` or :class:`ScoredPolygon` inferences.
-    :param Optional[List[Geometry]] ignored_ground_truths: optionally specify a list of :class:`BoundingBox` or
-        :class:`Polygon` ground truths to ignore. These ignored ground truths and any inferences matched with them are
-        omitted from the returned :class:`InferenceMatches`.
-    :param Literal["pascal"] mode: the type of matching methodology to use. See available modes above.
-    :param iou_threshold: the IOU (intersection over union, see :meth:`iou`) threshold for valid matches.
-    :return: :class:`InferenceMatches` containing the matches (true positives), unmatched ground truths (false
-        negatives) and unmatched inferences (false positives).
+    :param List[Geometry] ground_truths: A list of [`BoundingBox`][kolena.workflow.annotation.BoundingBox] or
+        [`Polygon`][kolena.workflow.annotation.Polygon] ground truths.
+    :param List[ScoredGeometry] inferences: A list of
+        [`ScoredBoundingBox`][kolena.workflow.annotation.ScoredBoundingBox] or
+        [`ScoredPolygon`][kolena.workflow.annotation.ScoredPolygon] inferences.
+    :param Optional[List[Geometry]] ignored_ground_truths: Optionally specify a list of
+        [`BoundingBox`][kolena.workflow.annotation.BoundingBox] or [`Polygon`][kolena.workflow.annotation.Polygon]
+        ground truths to ignore. These ignored ground truths and any inferences matched with them are
+        omitted from the returned [`InferenceMatches`][kolena.workflow.metrics.InferenceMatches].
+    :param mode: The matching methodology to use. See available modes above.
+    :param iou_threshold: The IOU (intersection over union, see [`iou`][kolena.workflow.metrics.iou]) threshold for
+        valid matches.
+    :return: [`InferenceMatches`][kolena.workflow.metrics.InferenceMatches] containing the matches (true positives),
+        unmatched ground truths (false negatives) and unmatched inferences (false positives).
     """
 
     if mode == "pascal":
         return _match_inferences_single_class_pascal_voc(
             ground_truths,
             inferences,
             ignored_ground_truths=ignored_ground_truths,
@@ -206,69 +215,80 @@
 GT_Multiclass = TypeVar("GT_Multiclass", bound=Union[LabeledBoundingBox, LabeledPolygon])
 Inf_Multiclass = TypeVar("Inf_Multiclass", bound=Union[ScoredLabeledBoundingBox, ScoredLabeledPolygon])
 
 
 @dataclass(frozen=True)
 class MulticlassInferenceMatches(Generic[GT_Multiclass, Inf_Multiclass]):
     """
-    The result of :func:`match_inferences_multiclass`, providing lists of matches between ground truth and inference
-    objects, unmatched ground truths, and unmatched inferences. The unmatched ground truths may be matched with an
-    inference of a different class when no inference of its own class is suitable, a confused match.
-    :class:`MultiClassInferenceMatches` can be used to calculate metrics such as precision and recall per class, after
-    applying some confidence threshold on the returned inference objects.
+    The result of [`match_inferences_multiclass`][kolena.workflow.metrics.match_inferences_multiclass], providing lists
+    of matches between ground truth and inference objects, unmatched ground truths, and unmatched inferences.
 
-    Objects are of type :class:`BoundingBox` or :class:`Polygon`, depending on the type of inputs provided to
-    :func:`match_inferences`.
+    Unmatched ground truths may be matched with an inference of a different class when no inference of its own class is
+    suitable, i.e. a "confused" match. `MultiClassInferenceMatches` can be used to calculate metrics such as precision
+    and recall per class, after applying some confidence threshold on the returned inference objects.
+
+    Objects are of type [`LabeledBoundingBox`][kolena.workflow.annotation.LabeledBoundingBox] or
+    [`LabeledPolygon`][kolena.workflow.annotation.LabeledPolygon], depending on the type of inputs provided to
+    [`match_inferences_multiclass`][kolena.workflow.metrics.match_inferences_multiclass].
     """
 
-    #: Pairs of matched ground truth and inference objects above the IOU threshold. Considered as true positive
-    #: detections after applying some confidence threshold.
     matched: List[Tuple[GT_Multiclass, Inf_Multiclass]]
+    """
+    Pairs of matched ground truth and inference objects above the IOU threshold. Considered as true positive
+    detections after applying some confidence threshold.
+    """
 
-    #: Pairs of unmatched ground truth objects with its confused inference object (i.e. IOU above threshold with
-    # mismatching ``label``), if such an inference exists. Considered as false negatives and "confused" detections.
     unmatched_gt: List[Tuple[GT_Multiclass, Optional[Inf_Multiclass]]]
+    """
+    Pairs of unmatched ground truth objects with its confused inference object (i.e. IOU above threshold with
+    mismatching `label`), if such an inference exists. Considered as false negatives and "confused" detections.
+    """
 
-    #: Unmatched inference objects. Considered as false positives after applying some confidence threshold.
     unmatched_inf: List[Inf_Multiclass]
+    """Unmatched inference objects. Considered as false positives after applying some confidence threshold."""
 
 
 def match_inferences_multiclass(
     ground_truths: List[GT_Multiclass],
     inferences: List[Inf_Multiclass],
     *,
     ignored_ground_truths: Optional[List[GT_Multiclass]] = None,
     mode: Literal["pascal"] = "pascal",
     iou_threshold: float = 0.5,
 ) -> MulticlassInferenceMatches[GT_Multiclass, Inf_Multiclass]:
     """
     Matches model inferences with annotated ground truths using the provided configuration.
 
-    This matcher considers ``label`` values matching per class. After matching inferences and ground truths with
-    equivalent ``label`` values, unmatched inferences and unmatched ground truths are matched once more to identify
-    confused matches, where localization succeeded (i.e. IOU above ``iou_threshold``) but classification failed (i.e.
-    mismatching ``label`` values).
+    This matcher considers `label` values matching per class. After matching inferences and ground truths with
+    equivalent `label` values, unmatched inferences and unmatched ground truths are matched once more to identify
+    confused matches, where localization succeeded (i.e. IOU above `iou_threshold`) but classification failed (i.e.
+    mismatching `label` values).
 
     Available modes:
 
-    - ``pascal`` (PASCAL VOC): For every inference by order of highest confidence, the ground truth of highest IOU is
+    - `pascal` (PASCAL VOC): For every inference by order of highest confidence, the ground truth of highest IOU is
       its match. Multiple inferences are able to match with the same ignored ground truth. See the
-      `PASCAL VOC paper <https://homepages.inf.ed.ac.uk/ckiw/postscript/ijcv_voc09.pdf>`_ for more information.
+      [PASCAL VOC paper](https://homepages.inf.ed.ac.uk/ckiw/postscript/ijcv_voc09.pdf) for more information.
 
-    :param List[LabeledGeometry] ground_truths: a list of :class:`LabeledBoundingBox` or :class:`LabeledPolygon` ground
-        truths.
-    :param List[ScoredLabeledGeometry] inferences: a list of :class:`ScoredLabeledBoundingBox` or
-        :class:`ScoredLabeledPolygon` inferences.
-    :param Optional[List[LabeledGeometry]] ignored_ground_truths: optionally specify a list of
-        :class:`LabeledBoundingBox` or :class:`LabeledPolygon` ground truths to ignore. These ignored ground truths any
-        any inferences matched with them are omitted from the returned :class:`MulticlassInferenceMatches`.
-    :param Literal["pascal"] mode: The type of matching methodology to use. See available modes above.
+    :param List[LabeledGeometry] ground_truths: A list of
+        [`LabeledBoundingBox`][kolena.workflow.annotation.LabeledBoundingBox] or
+        [`LabeledPolygon`][kolena.workflow.annotation.LabeledPolygon] ground truths.
+    :param List[ScoredLabeledGeometry] inferences: A list of
+        [`ScoredLabeledBoundingBox`][kolena.workflow.annotation.ScoredLabeledBoundingBox] or
+        [`ScoredLabeledPolygon`][kolena.workflow.annotation.ScoredLabeledPolygon] inferences.
+    :param Optional[List[LabeledGeometry]] ignored_ground_truths: Optionally specify a list of
+        [`LabeledBoundingBox`][kolena.workflow.annotation.LabeledBoundingBox] or
+        [`LabeledPolygon`][kolena.workflow.annotation.LabeledPolygon] ground truths to ignore. These ignored ground
+        truths and any inferences matched with them are omitted from the returned
+        [`MulticlassInferenceMatches`][kolena.workflow.metrics.MulticlassInferenceMatches].
+    :param mode: The matching methodology to use. See available modes above.
     :param iou_threshold: The IOU threshold cutoff for valid matches.
-    :return: :class:`MulticlassInferenceMatches` containing the matches (true positives), unmatched ground truths (false
-        negatives), and unmatched inferences (false positives).
+    :return:
+        [`MulticlassInferenceMatches`][kolena.workflow.metrics.MulticlassInferenceMatches] containing the matches
+        (true positives), unmatched ground truths (false negatives), and unmatched inferences (false positives).
     """
     matched: List[Tuple[GT_Multiclass, Inf_Multiclass]] = []
     unmatched_gt: List[GT_Multiclass] = []
     unmatched_inf: List[Inf_Multiclass] = []
     gts_by_class: Dict[str, List[GT_Multiclass]] = defaultdict(list)
     infs_by_class: Dict[str, List[Inf_Multiclass]] = defaultdict(list)
     ignored_gts_by_class: Dict[str, List[GT_Multiclass]] = defaultdict(list)
```

### Comparing `kolena_client-0.72.0/kolena/workflow/model.py` & `kolena_client-0.73.0/kolena/workflow/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,31 +47,42 @@
 from kolena.workflow.workflow import Workflow
 
 
 TestSample = TypeVar("TestSample", bound=BaseTestSample)
 
 
 class Model(Frozen, WithTelemetry, metaclass=ABCMeta):
-    """The descriptor of a model tested on Kolena."""
+    """
+    The descriptor of a model tested on Kolena. A model is a deterministic transformation from
+    [`TestSample`][kolena.workflow.TestSample] inputs to [`Inference`][kolena.workflow.Inference] outputs.
+
+    Rather than importing this class directly, use the `Model` type definition returned from
+    [`define_workflow`][kolena.workflow.define_workflow.define_workflow].
+    """
 
-    #: The :class:`kolena.workflow.Workflow` of this model.
     workflow: Workflow
+    """
+    The workflow of this model. Automatically populated when constructing via the model type returned from
+    [`define_workflow`][kolena.workflow.define_workflow.define_workflow].
+    """
 
-    _id: int
-
-    #: Unique name of the model.
     name: str
+    """Unique name of the model."""
 
-    #: Unstructured metadata associated with the model.
     metadata: Dict[str, Any]
+    """Unstructured metadata associated with the model."""
 
-    #: Function transforming a :class:`kolena.workflow.TestSample` for a workflow into an
-    #: :class:`kolena.workflow.Inference` object. Required when using :meth:`kolena.workflow.test` or
-    #: :meth:`kolena.workflow.TestRun.run`.
     infer: Optional[Callable[[TestSample], Inference]]
+    """
+    Function transforming a [`TestSample`][kolena.workflow.TestSample] for a workflow into an
+    [`Inference`][kolena.workflow.Inference] object. Required when using [`test`][kolena.workflow.test] or
+    [`TestRun.run`][kolena.workflow.TestRun.run].
+    """
+
+    _id: int
 
     @telemetry
     def __init_subclass__(cls) -> None:
         if not hasattr(cls, "workflow"):
             raise NotImplementedError(f"{cls.__name__} must implement class attribute 'workflow'")
         super().__init_subclass__()
 
@@ -87,75 +98,71 @@
         try:
             loaded = self.load(name, infer)
             if len(loaded.metadata.keys()) > 0 and loaded.metadata != metadata:
                 log.warn(f"mismatch in model metadata, using loaded metadata (loaded: {loaded.metadata})")
         except NotFoundError:
             loaded = self.create(name, infer, metadata)
 
-        self._id = loaded._id
-        self.name = loaded.name
-        self.metadata = loaded.metadata
-        self.infer = infer
-        self._freeze()
+        self._populate_from_other(loaded)
 
     @classmethod
     def create(
         cls,
         name: str,
         infer: Optional[Callable[[TestSample], Inference]] = None,
         metadata: Optional[Dict[str, Any]] = None,
     ) -> "Model":
         """
         Create a new model.
 
-        :param name: the unique name of the new model to create.
-        :param infer: optional inference function for this model.
-        :param metadata: optional unstructured metadata to store with this model.
-        :return: the newly created model.
+        :param name: The unique name of the new model to create.
+        :param infer: Optional inference function for this model.
+        :param metadata: Optional unstructured metadata to store with this model.
+        :return: The newly created model.
         """
         metadata = metadata or {}
         request = CoreAPI.CreateRequest(name=name, metadata=metadata, workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
         log.info(f"created model '{name}' ({get_model_url(obj._id)})")
         return obj
 
     @classmethod
     def load(cls, name: str, infer: Optional[Callable[[TestSample], Inference]] = None) -> "Model":
         """
         Load an existing model.
 
-        :param name: the name of the model to load.
-        :param infer: optional inference function for this model.
+        :param name: The name of the model to load.
+        :param infer: Optional inference function for this model.
         """
         request = CoreAPI.LoadByNameRequest(name=name)
         res = krequests.put(endpoint_path=API.Path.LOAD.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
         log.info(f"loaded model '{name}' ({get_model_url(obj._id)})")
         return obj
 
     @validate_arguments(config=ValidatorConfig)
     def load_inferences(self, test_case: TestCase) -> List[Tuple[TestSample, GroundTruth, Inference]]:
         """
         Load all inferences stored for this model on the provided test case.
 
-        :param test_case: the test case for which to load inferences.
-        :return: the ground truths and inferences for all test samples in the test case.
+        :param test_case: The test case for which to load inferences.
+        :return: The ground truths and inferences for all test samples in the test case.
         """
         return list(self.iter_inferences(test_case))
 
     @validate_arguments(config=ValidatorConfig)
     def iter_inferences(self, test_case: TestCase) -> Iterator[Tuple[TestSample, GroundTruth, Inference]]:
         """
         Iterate over all inferences stored for this model on the provided test case.
 
-        :param test_case: the test case over which to iterate inferences.
-        :return: an iterator exposing the ground truths and inferences for all test samples in the test case.
+        :param test_case: The test case over which to iterate inferences.
+        :return: Iterator exposing the ground truths and inferences for all test samples in the test case.
         """
         log.info(f"loading inferences from model '{self.name}' on test case '{test_case.name}'")
         assert_workflows_match(self.workflow.name, test_case.workflow.name)
         for df_batch in _BatchedLoader.iter_data(
             init_request=API.LoadInferencesRequest(
                 model_id=self._id,
                 test_case_id=test_case._id,
@@ -167,14 +174,22 @@
             for record in df_batch.itertuples():
                 test_sample = self.workflow.test_sample_type._from_dict(record.test_sample)
                 ground_truth = self.workflow.ground_truth_type._from_dict(record.ground_truth)
                 inference = self.workflow.inference_type._from_dict(record.inference)
                 yield test_sample, ground_truth, inference
         log.info(f"loaded inferences from model '{self.name}' on test case '{test_case.name}'")
 
+    def _populate_from_other(self, other: "Model") -> None:
+        with self._unfrozen():
+            self._id = other._id
+            self.name = other.name
+            self.metadata = other.metadata
+            self.workflow = other.workflow
+            self.infer = other.infer
+
     @classmethod
     def _from_data_with_infer(
         cls,
         data: CoreAPI.EntityData,
         infer: Optional[Callable[[TestSample], Inference]] = None,
     ) -> "Model":
         assert_workflows_match(cls.workflow.name, data.workflow)
```

### Comparing `kolena_client-0.72.0/kolena/workflow/test_case.py` & `kolena_client-0.73.0/kolena/workflow/test_case.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,30 +45,40 @@
 from kolena.workflow._datatypes import TestSampleDataFrame
 from kolena.workflow._validators import assert_workflows_match
 from kolena.workflow.test_sample import _METADATA_KEY
 from kolena.workflow.workflow import Workflow
 
 
 class TestCase(Frozen, WithTelemetry, metaclass=ABCMeta):
-    """A test case holds a set of images to compute aggregate performance metrics against."""
+    """
+    A test case holds a list of [test samples][kolena.workflow.TestSample] paired with
+    [ground truths][kolena.workflow.GroundTruth] representing a testing dataset or a slice of a testing dataset.
+
+    Rather than importing this class directly, use the `TestCase` type definition returned from
+    [`define_workflow`][kolena.workflow.define_workflow.define_workflow].
+    """
 
-    #: The :class:`kolena.workflow.Workflow` of this test case.
     workflow: Workflow
+    """
+    The workflow of this test case. Automatically populated when constructing via test case type returned from
+    [`define_workflow`][kolena.workflow.define_workflow.define_workflow].
+    """
 
-    _id: int
-
-    #: The unique name of this test case. Cannot be changed after creation.
     name: str
+    """The unique name of this test case. Cannot be changed after creation."""
 
-    #: The version of this test case. A test case's version is automatically incremented whenever it is edited via
-    #: :meth:`TestCase.edit`.
     version: int
+    """The version of this test case. A test case's version is automatically incremented whenever it is edited via
+    [`TestCase.edit`][kolena.workflow.TestCase.edit]."""
 
-    #: Free-form, human-readable description of this test case. Can be edited at any time via :meth:`TestCase.edit`.
     description: str
+    """Free-form, human-readable description of this test case. Can be edited at any time via
+    [`TestCase.edit`][kolena.workflow.TestCase.edit]."""
+
+    _id: int
 
     @telemetry
     def __init_subclass__(cls) -> None:
         if not hasattr(cls, "workflow"):
             raise NotImplementedError(f"{cls.__name__} must implement class attribute 'workflow'")
         super().__init_subclass__()
 
@@ -147,18 +157,18 @@
         name: str,
         description: Optional[str] = None,
         test_samples: Optional[List[Tuple[TestSample, GroundTruth]]] = None,
     ) -> "TestCase":
         """
         Create a new test case with the provided name.
 
-        :param name: the name of the new test case to create.
-        :param description: optional free-form description of the test case to create.
-        :param test_samples: optionally specify a set of test samples and ground truths to populate the test case.
-        :return: the newly created test case.
+        :param name: The name of the new test case to create.
+        :param description: Optional free-form description of the test case to create.
+        :param test_samples: Optionally specify a set of test samples and ground truths to populate the test case.
+        :return: The newly created test case.
         """
         cls._validate_test_samples(test_samples)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
@@ -168,32 +178,42 @@
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
         Load an existing test case with the provided name.
 
-        :param name: the name of the test case to load.
-        :param version: optionally specify a particular version of the test case to load. Defaults to the latest version
+        :param name: The name of the test case to load.
+        :param version: Optionally specify a particular version of the test case to load. Defaults to the latest version
             when unset.
-        :return: the loaded test case.
+        :return: The loaded test case.
         """
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         log.info(f"loaded test case '{name}' (v{data.version})")
         return cls._create_from_data(data)
 
     def load_test_samples(self) -> List[Tuple[TestSample, GroundTruth]]:
-        """Load all test samples and ground truths in this test case."""
+        """
+        Load all [`TestSample`s][kolena.workflow.TestSample] and [`GroundTruth`s][kolena.workflow.GroundTruth] contained
+        in this test case.
+
+        :return: A list of each test sample, paired with its ground truth, in this test case.
+        """
         return list(self.iter_test_samples())
 
     def iter_test_samples(self) -> Iterator[Tuple[TestSample, GroundTruth]]:
-        """Iterate through all test samples and ground truths in this test case."""
+        """
+        Iterate through all [`TestSample`s][kolena.workflow.TestSample] and
+        [`GroundTruth`s][kolena.workflow.GroundTruth] contained in this test case.
+
+        :return: An iterator yielding each test sample, paired with its ground truth, in this test case.
+        """
         log.info(f"loading test samples in test case '{self.name}' (v{self.version})")
         test_sample_type = self.workflow.test_sample_type
         ground_truth_type = self.workflow.ground_truth_type
         init_request = CoreAPI.InitLoadContentsRequest(batch_size=BatchSize.LOAD_SAMPLES.value, test_case_id=self._id)
         for df in _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_TEST_SAMPLES.value,
@@ -233,25 +253,25 @@
 
         @validate_arguments(config=ValidatorConfig)
         def add(self, test_sample: TestSample, ground_truth: GroundTruth) -> None:
             """
             Add a test sample to the test case. When the test sample already exists in the test case, its ground truth
             is overwritten with the ground truth provided here.
 
-            :param test_sample: the test sample to add.
-            :param ground_truth: the ground truth for the test sample.
+            :param test_sample: The test sample to add.
+            :param ground_truth: The ground truth for the test sample.
             """
             self._edits.append(self._Edit(test_sample, ground_truth=ground_truth))
 
         @validate_arguments(config=ValidatorConfig)
         def remove(self, test_sample: TestSample) -> None:
             """
             Remove a test sample from the test case. Does nothing if the test sample is not in the test case.
 
-            :param test_sample: the test sample to remove.
+            :param test_sample: The test sample to remove.
             """
             self._edits.append(self._Edit(test_sample, remove=True))
 
         def _edited(self) -> bool:
             return len(self._edits) > 0 or self._reset or self._description != self._initial_description
 
         def _to_data_frame(self) -> TestCaseEditorDataFrame:
@@ -270,24 +290,24 @@
             return TestCaseEditorDataFrame(validate_df_schema(df, TestCaseEditorDataFrame.get_schema(), trusted=True))
 
     @contextmanager
     def edit(self, reset: bool = False) -> Iterator[Editor]:
         """
         Edit this test case in a context:
 
-        .. code-block:: python
-
-            with test_case.edit() as editor:
-                # perform as many editing actions as desired
-                editor.add(...)
-                editor.remove(...)
+        ```python
+        with test_case.edit() as editor:
+            # perform as many editing actions as desired
+            editor.add(...)
+            editor.remove(...)
+        ```
 
         Changes are committed to the Kolena platform when the context is exited.
 
-        :param reset: clear any and all test samples currently in the test case.
+        :param reset: Clear any and all test samples currently in the test case.
         """
         editor = self.Editor(self.description, reset)
 
         yield editor
 
         if not editor._edited():
             return
```

### Comparing `kolena_client-0.72.0/kolena/workflow/test_run.py` & `kolena_client-0.73.0/kolena/workflow/test_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,44 +68,33 @@
 from kolena.workflow.evaluator_function import _TestCases
 from kolena.workflow.evaluator_function import BasicEvaluatorFunction
 from kolena.workflow.evaluator_function import EvaluationResults
 
 
 class TestRun(Frozen, WithTelemetry, metaclass=ABCMeta):
     """
-    A :class:`kolena.workflow.Model` tested on a :class:`kolena.workflow.TestSuite` using a specific
-    :class:`kolena.workflow.Evaluator` implementation.
+    A [`Model`][kolena.workflow.Model] tested on a [`TestSuite`][kolena.workflow.TestSuite] using a specific
+    [`Evaluator`][kolena.workflow.Evaluator] implementation.
 
-    :param model: the model being tested.
-    :param test_suite: the test suite on which to test the model.
-    :param Union[Evaluator, BasicEvaluatorFunction, None] evaluator: an optional evaluator implementation.
+    :param model: The model being tested.
+    :param test_suite: The test suite on which to test the model.
+    :param evaluator: An optional evaluator implementation.
         Requires a previously configured server-side evaluator to default to if omitted.
-        (Please see :class:`kolena.workflow.BasicEvaluatorFunction` for type definition.)
+        (Please see [`BasicEvaluatorFunction`][kolena.workflow.evaluator_function.BasicEvaluatorFunction] for type
+        definition.)
     :param configurations: a list of configurations to use when running the evaluator.
     :param reset: overwrites existing inferences if set.
     """
 
     _id: int
 
     model: Model
-    """
-    :meta private:
-    """
     test_suite: TestSuite
-    """
-    :meta private:
-    """
     evaluator: Union[Evaluator, BasicEvaluatorFunction, None]
-    """
-    :meta private:
-    """
     configurations: Optional[List[EvaluatorConfiguration]]
-    """
-    :meta private:
-    """
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(
         self,
         model: Model,
         test_suite: TestSuite,
         evaluator: Union[Evaluator, BasicEvaluatorFunction, None] = None,
@@ -246,15 +235,15 @@
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(res)
 
     def evaluate(self) -> None:
         """
         Perform evaluation by computing metrics for individual test samples, in aggregate across test cases, and across
-        the complete test suite at each :class:`kolena.workflow.EvaluatorConfiguration`.
+        the complete test suite at each [`EvaluatorConfiguration`][kolena.workflow.EvaluatorConfiguration].
         """
         if self.evaluator is None:
             log.info("commencing server side metrics evaluation")
             self._start_server_side_evaluation()
             return
 
         # TODO: assert that testing is complete?
@@ -487,19 +476,26 @@
     model: Model,
     test_suite: TestSuite,
     evaluator: Union[Evaluator, BasicEvaluatorFunction, None] = None,
     configurations: Optional[List[EvaluatorConfiguration]] = None,
     reset: bool = False,
 ) -> None:
     """
-    Test a :class:`kolena.workflow.Model` on a :class:`kolena.workflow.TestSuite` using a specific
-    :class:`kolena.workflow.Evaluator` or :class:`kolena.workflow.StreamlinedEvaluator` implementation.
+    Test a [`Model`][kolena.workflow.Model] on a [`TestSuite`][kolena.workflow.TestSuite] using a specific
+    [`Evaluator`][kolena.workflow.Evaluator] implementation.
+
+    ```python
+    from kolena.workflow import test
 
-    :param model: the model being tested, implementing the ``infer`` method.
-    :param test_suite: the test suite on which to test the model.
-    :param Union[Evaluator, BasicEvaluatorFunction, None] evaluator: an optional evaluator implementation.
+    test(model, test_suite, evaluator, reset=True)
+    ```
+
+    :param model: The model being tested, implementing the `infer` method.
+    :param test_suite: The test suite on which to test the model.
+    :param evaluator: An optional evaluator implementation.
         Requires a previously configured server-side evaluator to default to if omitted.
-        (Please see :class:`kolena.workflow.BasicEvaluatorFunction` for type definition.)
-    :param configurations: a list of configurations to use when running the evaluator.
-    :param reset: overwrites existing inferences if set.
+        (Please see [`BasicEvaluatorFunction`][kolena.workflow.evaluator_function.BasicEvaluatorFunction] for type
+        definition.)
+    :param configurations: A list of configurations to use when running the evaluator.
+    :param reset: Overwrites existing inferences if set.
     """
     TestRun(model, test_suite, evaluator, configurations, reset).run()
```

### Comparing `kolena_client-0.72.0/kolena/workflow/test_sample.py` & `kolena_client-0.73.0/kolena/workflow/test_sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,35 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+Test samples are the inputs to your models when testing.
+
+For example, for a model that processes specific regions within a larger image, its test sample may be defined:
+
+```python
+from dataclasses import dataclass
+
+from kolena.workflow import Image
+from kolena.workflow.annotation import BoundingBox
+
+@dataclass(frozen=True)
+class ImageWithRegion(Image):
+    region: BoundingBox
+
+example = ImageWithRegion(
+    locator="s3://my-bucket/example-image.png",  # field from Image base class
+    region=BoundingBox(top_left=(0, 0), bottom_right=(100, 100)),
+)
+```
+"""
 import copy
 from abc import ABCMeta
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
@@ -31,17 +52,14 @@
 from kolena.workflow._datatypes import TypedDataObject
 from kolena.workflow._validators import get_data_object_field_types
 from kolena.workflow._validators import safe_issubclass
 from kolena.workflow._validators import validate_field
 from kolena.workflow._validators import validate_metadata_dict
 from kolena.workflow.asset import ImageAsset
 
-#: Type of the ``metadata`` field that can be included on :class:`kolena.workflow.TestSample` definitions. String
-#: (``str``) keys and scalar values (``int``, ``float``, ``str``, ``bool``, ``None``) as well as scalar list values are
-#: permitted.
 Metadata = Dict[
     str,
     Union[
         None,
         # prevent coercion of values in metadata -- see: https://pydantic-docs.helpmanual.io/usage/types/#strict-types
         StrictStr,
         StrictFloat,
@@ -64,14 +82,28 @@
                 float,
                 int,
                 bool,
             ]
         ],
     ],
 ]
+"""
+Type of the `metadata` field that can be included on [`TestSample`][kolena.workflow.TestSample] definitions. String
+(`str`) keys and scalar values (`int`, `float`, `str`, `bool`, `None`) as well as scalar list values are permitted.
+
+```python
+from dataclasses import dataclass, field
+from kolena.workflow import Image, Metadata
+
+@dataclass(frozen=True)
+class ImageWithMetadata(Image):
+    metadata: Metadata = field(default_factory=dict)
+```
+"""
+
 _METADATA_KEY = "metadata"
 
 
 class _TestSampleType(DataType):
     IMAGE = "IMAGE"
     TEXT = "TEXT"
     VIDEO = "VIDEO"
@@ -88,23 +120,23 @@
 class TestSample(TypedDataObject[_TestSampleType], metaclass=ABCMeta):
     """
     The inputs to a model.
 
     Test samples can be customized as necessary for a workflow by extending this class or one of the built-in test
     sample types.
 
-    Extensions to the ``TestSample`` class may define a ``metadata`` field of type
-    :data:`kolena.workflow.test_sample.Metadata` containing a dictionary of scalar properties associated with the test
-    sample, intended for use when sorting or filtering test samples.
+    Extensions to the `TestSample` class may define a `metadata` field of type
+    [`Metadata`][kolena.workflow.test_sample.Metadata] containing a dictionary of scalar properties associated with the
+    test sample, intended for use when sorting or filtering test samples.
 
-    Kolena handles the ``metadata`` field differently from other test sample fields. Updates to the ``metadata`` object
-    for a given test sample are merged with previously uploaded metadata. As such, ``metadata`` for a given test sample
+    Kolena handles the `metadata` field differently from other test sample fields. Updates to the `metadata` object
+    for a given test sample are merged with previously uploaded metadata. As such, `metadata` for a given test sample
     within a test case is **not** immutable, and should **not** be relied on when an implementation of
-    :class:`kolena.workflow.Model` computes inferences, or when an implementation of :class:`kolena.workflow.Evaluator`
-    evaluates metrics.
+    [`Model`][kolena.workflow.Model] computes inferences, or when an implementation of
+    [`Evaluator`][kolena.workflow.Evaluator] evaluates metrics.
     """
 
     @staticmethod
     def _data_type() -> _TestSampleType:
         return _TestSampleType.CUSTOM
 
     def _to_dict(self) -> Dict[str, Any]:
@@ -116,112 +148,123 @@
         base_dict = super()._to_dict()
         return base_dict.pop(_METADATA_KEY, {})
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Composite(TestSample):
     """
-    A test sample composed of multiple basic :class:`TestSample` elements.
+    A test sample composed of multiple basic [`TestSample`][kolena.workflow.TestSample] elements.
 
     An example application would be each test sample is a pair of face images, and the goal is to predict whether the
     two images are of the same person. For this use-case the test sample can be defined as:
 
-    .. code-block:: python
-
-        class FacePairSample(Composite):
-            source: Image
-            target: Image
+    ```python
+    class FacePairSample(Composite):
+        source: Image
+        target: Image
+    ```
 
-    To facilitate visualization for this kind of use cases, see usage of :class:`kolena.workflow.GroundTruth` and
-    :class:`kolena.workflow.Inference`.
+    To facilitate visualization for this kind of use cases, see usage of [`GroundTruth`][kolena.workflow.GroundTruth]
+    and [`Inference`][kolena.workflow.Inference].
     """
 
     @classmethod
     def _data_type(cls) -> _TestSampleType:
         return _TestSampleType.COMPOSITE
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Image(TestSample):
     """An image located in a cloud bucket or served at a URL."""
 
     locator: str
+    """The URL of this image, using e.g. `s3`, `gs`, or `https` scheme (`s3://my-bucket/path/to/image.png`)."""
 
     @classmethod
     def _data_type(cls) -> _TestSampleType:
         return _TestSampleType.IMAGE
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ImagePair(Composite):
-    """Two images."""
+    """Two [`Image`s][kolena.workflow.Image] paired together."""
 
     a: Image
+    """The left [`Image`][kolena.workflow.Image] in the image pair."""
+
     b: Image
+    """The right [`Image`][kolena.workflow.Image] in the image pair."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Text(TestSample):
-    """A text snippet."""
+    """An inline text snippet."""
 
     text: str
+    """The text snippet."""
 
     @classmethod
     def _data_type(cls) -> _TestSampleType:
         return _TestSampleType.TEXT
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class ImageText(Composite):
     """An image paired with a text snippet."""
 
     image: Image
+    """The [`Image`][kolena.workflow.Image] in this image-text pair."""
+
     text: Text
+    """The text snippet in this image-text pair."""
 
 
 # NOTE: declare BaseVideo as separate class for extension -- default fields in main Video class prevent extension with
 #  non-default fields
 @dataclass(frozen=True, config=ValidatorConfig)
 class BaseVideo(TestSample):
     """A video clip located in a cloud bucket or served at a URL."""
 
-    #: URL (e.g. S3, HTTPS) of the video file
     locator: str
+    """URL (e.g. S3, HTTPS) of the video file."""
 
     @classmethod
     def _data_type(cls) -> _TestSampleType:
         return _TestSampleType.VIDEO
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Video(BaseVideo):
     """A video clip located in a cloud bucket or served at a URL."""
 
-    #: Optionally provide asset locator for custom video thumbnail
+    locator: str
+    """URL (e.g. S3, HTTPS) of the video file."""
+
     thumbnail: Optional[ImageAsset] = None
+    """Optionally provide asset locator for custom video thumbnail."""
 
-    #: Optionally specify start time of video snippet, in seconds
     start: Optional[float] = None
+    """Optionally specify start time of video snippet, in seconds."""
 
-    #: Optionally specify end time of video snippet, in seconds
     end: Optional[float] = None
+    """Optionally specify end time of video snippet, in seconds."""
 
     def __post_init__(self) -> None:
         if self.start is not None and self.end is not None and self.start > self.end:
             raise ValueError(f"Specified start time '{self.start}' is after specified end time '{self.end}'")
         if self.start is not None and self.end is not None and (self.start < 0 or self.end < 0):
             raise ValueError(f"Specified start time '{self.start}' and end time '{self.end}' must be non-negative")
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Document(TestSample):
     """A remotely linked document, e.g. PDF or TXT file."""
 
-    #: URL (e.g. S3, HTTPS) of the document
     locator: str
+    """URL (e.g. S3, HTTPS) of the document."""
 
     @classmethod
     def _data_type(cls) -> _TestSampleType:
         return _TestSampleType.DOCUMENT
 
 
 _TEST_SAMPLE_BASE_TYPES = [Composite, Image, Text, BaseVideo, Document]
```

### Comparing `kolena_client-0.72.0/kolena/workflow/test_suite.py` & `kolena_client-0.73.0/kolena/workflow/test_suite.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,39 +45,50 @@
 from kolena.workflow._validators import assert_workflows_match
 from kolena.workflow.test_case import TestCase
 from kolena.workflow.workflow import Workflow
 
 
 class TestSuite(Frozen, WithTelemetry, metaclass=ABCMeta):
     """
-    A test suite groups together one or more test cases.
-    """
+    A test suite groups together one or more [test cases][kolena.workflow.TestCase]. Typically a test suite represents a
+    benchmark test dataset, with test cases representing different meaningful subsets, or slices, or this benchmark.
 
-    _test_case_type: Type[TestCase]
+    Rather than importing this class directly, use the `TestSuite` type definition returned from
+    [`define_workflow`][kolena.workflow.define_workflow.define_workflow].
+    """
 
-    #: The :class:`kolena.workflow.Workflow` of this test suite.
     workflow: Workflow
+    """
+    The workflow of this test suite. Automatically populated when constructing via test suite type returned from
+    [`define_workflow`][kolena.workflow.define_workflow.define_workflow].
+    """
 
-    _id: int
-
-    #: The unique name of this test suite. Cannot be changed after creation.
     name: str
+    """The unique name of this test suite."""
 
-    #: The version of this test suite. A test suite's version is automatically incremented whenever it is edited via
-    #: :meth:`TestSuite.edit`.
     version: int
+    """
+    The version of this test suite. A test suite's version is automatically incremented whenever it is edited via
+    [`TestSuite.edit`][kolena.workflow.TestSuite.edit].
+    """
 
-    #: Free-form, human-readable description of this test suite. Can be edited at any time via :meth:`TestSuite.edit`.
     description: str
+    """
+    Free-form, human-readable description of this test suite. Can be edited at any time via
+    [`TestSuite.edit`][kolena.workflow.TestSuite.edit].
+    """
 
-    #: The :class:`kolena.workflow.TestCase` objects belonging to this test suite.
     test_cases: List[TestCase]
+    """The [`TestCase`][kolena.workflow.TestCase] objects belonging to this test suite."""
 
-    #: The tags associated with this test suite.
     tags: Set[str]
+    """The tags associated with this test suite."""
+
+    _id: int
+    _test_case_type: Type[TestCase]
 
     @telemetry
     def __init_subclass__(cls) -> None:
         if not hasattr(cls, "workflow"):
             raise NotImplementedError(f"{cls.__name__} must implement class attribute 'workflow'")
         if not hasattr(cls, "_test_case_type"):
             raise NotImplementedError(f"{cls.__name__} must implement class attribute '_test_case_type'")
@@ -172,19 +183,19 @@
         description: Optional[str] = None,
         test_cases: Optional[List[TestCase]] = None,
         tags: Optional[Set[str]] = None,
     ) -> "TestSuite":
         """
         Create a new test suite with the provided name.
 
-        :param name: the name of the new test suite to create.
-        :param description: optional free-form description of the test suite to create.
-        :param test_cases: optionally specify a list of test cases to populate the test suite.
-        :param tags: optionally specify a set of tags to attach to the test suite.
-        :return: the newly created test suite.
+        :param name: The name of the new test suite to create.
+        :param description: Optional free-form description of the test suite to create.
+        :param test_cases: Optionally specify a list of test cases to populate the test suite.
+        :param tags: Optionally specify a set of tags to attach to the test suite.
+        :return: The newly created test suite.
         """
         cls._validate_workflow()
         cls._validate_test_cases(test_cases)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name, tags=tags)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
@@ -195,18 +206,18 @@
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         """
         Load an existing test suite with the provided name.
 
-        :param name: the name of the test suite to load.
-        :param version: optionally specify a particular version of the test suite to load. Defaults to the latest
+        :param name: The name of the test suite to load.
+        :param version: Optionally specify a particular version of the test suite to load. Defaults to the latest
             version when unset.
-        :return: the loaded test suite.
+        :return: The loaded test suite.
         """
         cls._validate_workflow()
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
@@ -214,18 +225,18 @@
         return obj
 
     @classmethod
     def load_all(cls, *, tags: Optional[Set[str]] = None) -> List["TestSuite"]:
         """
         Load the latest version of all non-archived test suites with this workflow.
 
-        :param tags: optionally specify a set of tags to apply as a filter. The loaded test suites will include only
+        :param tags: Optionally specify a set of tags to apply as a filter. The loaded test suites will include only
             test suites with tags matching each of these specified tags, i.e.
-            ``test_suite.tags.intersection(tags) == tags``.
-        :return: the latest version of all non-archived test suites, with matching tags when specified.
+            `test_suite.tags.intersection(tags) == tags`.
+        :return: The latest version of all non-archived test suites, with matching tags when specified.
         """
         cls._validate_workflow()
         request = CoreAPI.LoadAllRequest(workflow=cls.workflow.name, tags=tags)
         res = krequests.put(endpoint_path=API.Path.LOAD_ALL.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.LoadAllResponse, data=res.json())
         objs = [cls._create_from_data(test_suite) for test_suite in data.test_suites]
@@ -262,24 +273,24 @@
 
         @validate_arguments(config=ValidatorConfig)
         def add(self, test_case: TestCase) -> None:
             """
             Add a test case to this test suite. If a different version of the test case already exists in this test
             suite, it is replaced.
 
-            :param test_case: the test case to add to the test suite.
+            :param test_case: The test case to add to the test suite.
             """
             self._test_cases = [*(tc for tc in self._test_cases if tc.name != test_case.name), test_case]
 
         @validate_arguments(config=ValidatorConfig)
         def remove(self, test_case: TestCase) -> None:
             """
             Remove a test case from this test suite. Does nothing if the test case is not in the test suite.
 
-            :param test_case: the test case to remove.
+            :param test_case: The test case to remove.
             """
             self._test_cases = [tc for tc in self._test_cases if tc.name != test_case.name]
 
         def _edited(self) -> bool:
             return (
                 self._description != self._initial_description
                 or self._initial_test_case_ids != [tc._id for tc in self._test_cases]
@@ -287,24 +298,24 @@
             )
 
     @contextmanager
     def edit(self, reset: bool = False) -> Iterator[Editor]:
         """
         Edit this test suite in a context:
 
-        .. code-block:: python
-
-            with test_suite.edit() as editor:
-                # perform as many editing actions as desired
-                editor.add(...)
-                editor.remove(...)
+        ```python
+        with test_suite.edit() as editor:
+            # perform as many editing actions as desired
+            editor.add(...)
+            editor.remove(...)
+        ```
 
         Changes are committed to the Kolena platform when the context is exited.
 
-        :param reset: clear any and all test cases currently in the test suite.
+        :param reset: Clear any and all test cases currently in the test suite.
         """
         editor = self.Editor(self.test_cases, self.description, self.tags, reset)
 
         yield editor
 
         if not editor._edited():
             return
@@ -321,14 +332,20 @@
         res = krequests.post(endpoint_path=API.Path.EDIT, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         self._populate_from_other(self._create_from_data(test_suite_data))
         log.success(f"edited test suite '{self.name}' (v{self.version}) ({get_test_suite_url(self._id)})")
 
     def load_test_samples(self) -> List[Tuple[TestCase, List[TestSample]]]:
+        """
+        Load test samples for all test cases within this test suite.
+
+        :return: A list of [`TestCase`s][kolena.workflow.TestCase], each paired with the list of
+            [`TestSample`s][kolena.workflow.TestSample] it contains.
+        """
         test_case_id_to_samples: Dict[int, List[TestSample]] = defaultdict(list)
         for df_batch in _BatchedLoader.iter_data(
             init_request=API.LoadTestSamplesRequest(
                 test_suite_id=self._id,
                 batch_size=BatchSize.LOAD_SAMPLES,
             ),
             endpoint_path=API.Path.INIT_LOAD_TEST_SAMPLES,
```

### Comparing `kolena_client-0.72.0/kolena/workflow/workflow.py` & `kolena_client-0.73.0/kolena/workflow/workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,30 +86,28 @@
             secret=response.secret,
             aws_role_config=aws_role_config,
         )
 
 
 @dataclass(frozen=True)
 class Workflow:
-    """
-    The definition of a workflow and its associated types.
-    """
+    """The definition of a workflow and its associated types."""
 
-    #: The name of the workflow. Should be unique, meaningful, and human-readable.
     name: str
+    """The name of the workflow. Should be unique, meaningful, and human-readable."""
 
-    #: The :class:`kolena.workflow.TestSample` type for the workflow, using one of the builtin test sample types
-    #: (e.g. :class:`kolena.workflow.Image`) and extending as necessary with additional fields.
     test_sample_type: Type[TestSample]
+    """The [`TestSample`][kolena.workflow.TestSample] type for the workflow, using one of the builtin test sample types
+    (e.g. [`Image`][kolena.workflow.Image]) and extending as necessary with additional fields."""
 
-    #: The custom :class:`kolena.workflow.GroundTruth` type for the workflow.
     ground_truth_type: Type[GroundTruth]
+    """The custom [`GroundTruth`][kolena.workflow.GroundTruth] type for the workflow."""
 
-    #: The custom :class:`kolena.workflow.Inference` type for the workflow.
     inference_type: Type[Inference]
+    """The custom [`Inference`][kolena.workflow.Inference] type for the workflow."""
 
     def __post_init__(self) -> None:
         object.__setattr__(self, "name", self.name.strip())
         if self.name == "":
             raise ValueError("invalid zero-length name provided")
         if self.name.lower() in _RESERVED_WORKFLOW_NAMES:
             raise ValueError(f"invalid reserved name '{self.name}' provided")
@@ -123,32 +121,32 @@
         self,
         evaluator_name: str,
         image: str,
         secret: Optional[str] = None,
         aws_assume_role: Optional[str] = None,
     ) -> RemoteEvaluator:
         """
-        This is a convenience method to register evaluator for the workflow.
+        Convenience method to register evaluator for the workflow.
 
-        Please see :py:func:`register_evaluator` for details.
+        See [`register_evaluator`][kolena.workflow.workflow.register_evaluator] for details.
         """
         return register_evaluator(
             workflow=self.name,
             evaluator_name=evaluator_name,
             image=image,
             secret=secret,
             aws_assume_role=aws_assume_role,
         )
 
     @kolena_initialized
     def get_evaluator(self, evaluator_name: str, include_secret: bool = False) -> RemoteEvaluator:
         """
-        Get the docker image registered for the evaluator
+        Get the docker image registered for the evaluator.
 
-        Please see :py:func:`get_evaluator` for details.
+        See [`get_evaluator`][kolena.workflow.workflow.get_evaluator] for details.
         """
 
         return get_evaluator(self.name, evaluator_name, include_secret)
 
 
 @kolena_initialized
 def register_evaluator(
```

### Comparing `kolena_client-0.72.0/pyproject.toml` & `kolena_client-0.73.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.72.0"  # version is automatically set to latest git tag during release process
+version = "0.73.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
@@ -45,25 +45,35 @@
 retrying = "^1.3.3"
 Shapely = "^1.8.5"
 deprecation = "^2.1.0"
 termcolor = "^1.1.0"
 pyarrow = ">=8"
 typing-extensions = { version = "^4.5.0", python = "< 3.8" }
 click = "^8.1.3"
+scikit-learn = [
+    { version = ">=1.0,<1.0.3", python = ">=3.7.1,<3.8",  optional = true },
+    { version = ">=1.2", python = ">=3.8",  optional = true },
+]
+
+[tool.poetry.extras]
+metrics = ["scikit-learn"]
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.17"
-Sphinx = "^4.2.0"
-myst-parser = "^0.17"
-pydata-sphinx-theme = "^0.12"
-sphinx-autodoc-typehints = "^1.16.0"
 black = { version = "^22.1.0", allow-prereleases = true }
 pytest = "^7"
 pytest-cov = "^4.0.0"
 pytest-depends = "^1.0.1"
+mkdocs = "^1.4.3"
+cairosvg = "^2.7.0"
+mkdocs-material = "^9.1.15"  # insiders fork installed out-of-band in docs/setup_insiders.sh
+mkdocstrings = { version = ">0.20,<1", extras = ["python"] }
+mkdocs-git-committers-plugin-2 = "^1.1.2"
+mkdocs-git-revision-date-localized-plugin = "^1.2.0"
+mkdocs-glightbox = "^0.3.4"
 
 [tool.poetry.scripts]
 kolena = 'kolena._utils.cli:run'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -71,7 +81,10 @@
 [tool.pytest.ini_options]
 # do not scan 'kolena' for tests, as there are many functions/classes that look like tests
 norecursedirs = "kolena"
 # explicitly disable test classes such that e.g. TestRun is not interpreted as a test
 python_classes = []
 # only collect functions starting with 'test__'
 python_functions = ["test__*"]
+markers = [
+    "metrics: tests that extra dependencies for metrics",
+]
```

