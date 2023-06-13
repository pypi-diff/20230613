# Comparing `tmp/truss-0.4.8rc8.tar.gz` & `tmp/truss-0.4.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.8rc8.tar", max compression
+gzip compressed data, was "truss-0.4.9rc2.tar", max compression
```

## Comparing `truss-0.4.8rc8.tar` & `truss-0.4.9rc2.tar`

### file list

```diff
@@ -1,172 +1,178 @@
--rw-r--r--   0        0        0     5483 2023-06-07 20:46:27.144157 truss-0.4.8rc8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-06-07 20:46:27.144157 truss-0.4.8rc8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-06-07 20:46:27.144157 truss-0.4.8rc8/LICENSE
--rw-r--r--   0        0        0     5958 2023-06-07 20:46:27.144157 truss-0.4.8rc8/README.md
--rw-r--r--   0        0        0     3077 2023-06-07 20:46:27.144157 truss-0.4.8rc8/ROADMAP.md
--rw-r--r--   0        0        0      820 2023-06-07 20:46:27.144157 truss-0.4.8rc8/context_builder.Dockerfile
--rw-r--r--   0        0        0     2319 2023-06-07 20:46:27.260157 truss-0.4.8rc8/pyproject.toml
--rw-r--r--   0        0        0      330 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/build.py
--rw-r--r--   0        0        0    10452 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/cli.py
--rw-r--r--   0        0        0     2813 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/constants.py
--rw-r--r--   0        0        0     1294 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     8411 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1893 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2111 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/errors.py
--rw-r--r--   0        0        0      824 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6521 2023-06-07 20:46:27.260157 truss-0.4.8rc8/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/notebook.py
--rw-r--r--   0        0        0    11065 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/__init__.py
--rw-r--r--   0        0        0     1925 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1861 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       85 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1352 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     2382 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     3318 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     9426 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0     1445 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      727 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     6219 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      235 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     2769 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-06-07 20:46:27.264157 truss-0.4.8rc8/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1550 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/__init__.py
--rw-r--r--   0        0        0    20811 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    11109 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6931 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2252 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_build.py
--rw-r--r--   0        0        0     3181 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_docker.py
--rw-r--r--   0        0        0     4905 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    33902 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/tests/test_validation.py
--rw-r--r--   0        0        0    13164 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/truss_config.py
--rw-r--r--   0        0        0     2845 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/truss_gatherer.py
--rw-r--r--   0        0        0    40919 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/types.py
--rw-r--r--   0        0        0      227 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/util/jinja.py
--rw-r--r--   0        0        0     2018 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-06-07 20:46:27.268157 truss-0.4.8rc8/truss/validation.py
--rw-r--r--   0        0        0     7595 1970-01-01 00:00:00.000000 truss-0.4.8rc8/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-06-13 20:41:33.831349 truss-0.4.9rc2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-06-13 20:41:33.831349 truss-0.4.9rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-06-13 20:41:33.831349 truss-0.4.9rc2/LICENSE
+-rw-r--r--   0        0        0     5958 2023-06-13 20:41:33.831349 truss-0.4.9rc2/README.md
+-rw-r--r--   0        0        0     3077 2023-06-13 20:41:33.831349 truss-0.4.9rc2/ROADMAP.md
+-rw-r--r--   0        0        0      820 2023-06-13 20:41:33.835349 truss-0.4.9rc2/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2482 2023-06-13 20:41:33.939350 truss-0.4.9rc2/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/build.py
+-rw-r--r--   0        0        0    11326 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/cli.py
+-rw-r--r--   0        0        0     2813 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/constants.py
+-rw-r--r--   0        0        0     1294 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     8411 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1893 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2111 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     4715 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/local_server_loader.py
+-rw-r--r--   0        0        0     2239 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0      951 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/truss_file_syncer.py
+-rw-r--r--   0        0        0     5801 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6521 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/notebook.py
+-rw-r--r--   0        0        0    11065 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1925 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2503 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4272 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     3015 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2450 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     1352 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/logging.py
+-rw-r--r--   0        0        0     5389 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1875 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      126 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1352 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     2382 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     3318 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     9977 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0     1445 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      727 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0      496 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/local_inference_server.py
+-rw-r--r--   0        0        0     6219 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      250 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     2769 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0      739 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/__init__.py
+-rw-r--r--   0        0        0    20811 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    11109 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6977 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2252 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_build.py
+-rw-r--r--   0        0        0     3181 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     7062 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    33928 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    13164 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_config.py
+-rw-r--r--   0        0        0     2698 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41382 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/types.py
+-rw-r--r--   0        0        0      227 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/jinja.py
+-rw-r--r--   0        0        0     2612 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/validation.py
+-rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 truss-0.4.9rc2/PKG-INFO
```

### Comparing `truss-0.4.8rc8/CODE_OF_CONDUCT.md` & `truss-0.4.9rc2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/CONTRIBUTING.md` & `truss-0.4.9rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/LICENSE` & `truss-0.4.9rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/README.md` & `truss-0.4.9rc2/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/ROADMAP.md` & `truss-0.4.9rc2/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/context_builder.Dockerfile` & `truss-0.4.9rc2/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/pyproject.toml` & `truss-0.4.9rc2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.8rc8"
+version = "0.4.9rc2"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
@@ -30,14 +30,17 @@
 cloudpickle = "^2.2.0"
 blake3 = "^0.3.3"
 fastapi = "^0.95.0"
 uvicorn = "^0.21.1"
 psutil = "^5.9.4"
 joblib = "^1.2.0"
 dockerfile = "^3.2.0"
+virtualenv = "^20.23.0"
+watchfiles = "^0.19.0"
+yaspin = "^2.3.0"
 
 [tool.poetry.group.builder.dependencies]
 python = ">=3.8,<3.12"
 packaging = "^20.9"
 python-json-logger = ">=2.0.2"
 PyYAML = "^6.0"
 Jinja2 = "^3.1.2"
@@ -46,14 +49,18 @@
 single-source = "^0.3.0"
 click = "^8.0.3"
 requests = "^2.28.1"
 blake3 = "^0.3.3"
 fastapi = "^0.95.0"
 uvicorn = "^0.21.1"
 psutil = "^5.9.4"
+dockerfile = "^3.2.0"
+virtualenv = "^20.23.0"
+watchfiles = "^0.19.0"
+yaspin = "^2.3.0"
 
 [tool.poetry.dev-dependencies]
 torch = "^1.9.0"
 ipython = "^7.16"
 pytest = "7.2.0"
 tensorflow = { version = "^2.4.4", markers = "sys_platform == 'linux'" }
 tensorflow-macos = { version = "^2.4.4", markers = "sys_platform == 'darwin'" }
@@ -66,26 +73,25 @@
 ipdb = "^0.13.9"
 coverage = "^6.4.1"
 pytest-cov = "^3.0.0"
 xgboost = "^1.6.1"
 lightgbm = "^3.3.2"
 transformers = "^4.20.1"
 black = "^22.6.0"
-Flask = "^2.2.2"
-waitress = "^2.1.2"
 nbconvert = "^7.2.1"
 ipykernel = "^6.16.0"
 
 [tool.poetry.scripts]
 truss = 'truss.cli:cli_group'
 
 [tool.poetry.group.dev.dependencies]
 mlflow = "^1.29.0"
 mypy = "^1.0.0"
 pytest-split = "^0.8.1"
+httpx = {extras = ["cli"], version = "^0.24.1"}
 
 [build-system]
 requires = ["poetry-core>=1.2.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `truss-0.4.8rc8/truss/blob/blob_backend_registry.py` & `truss-0.4.9rc2/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/blob/http_public_blob_backend.py` & `truss-0.4.9rc2/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/build.py` & `truss-0.4.9rc2/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/cli.py` & `truss-0.4.9rc2/truss/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -147,14 +147,42 @@
         click.confirm(
             f"Container already exists at {urls}. Are you sure you want to continue?"
         )
     tr.docker_run(build_dir=build_dir, tag=tag, local_port=port, detach=not attach)
 
 
 @cli_group.command()
+@click.argument("target_directory", required=False)
+@click.option("--build-dir", type=Path, required=False)
+@click.option("--venv-dir", type=Path, required=False)
+@click.option("--port", type=int, default=8080, help="Local port used to run server")
+@error_handling
+def watch(
+    target_directory: str,
+    build_dir: Optional[Path],
+    venv_dir: Optional[Path],
+    port: int,
+) -> None:
+    """
+    Runs the model server for a Truss.
+
+    TARGET_DIRECTORY: A Truss directory. If none, use current directory.
+
+    BUILD_DIR: Image context. If none, a temp directory is created.
+    """
+    if build_dir:
+        build_dir = Path(build_dir)
+
+    if venv_dir:
+        venv_dir = Path(venv_dir)
+    tr = _get_truss_from_directory(target_directory=target_directory)
+    tr.run_local_server_with_reload(build_dir=build_dir, work_dir=venv_dir, port=port)
+
+
+@cli_group.command()
 @click.option("--target_directory", required=False, help="Directory of truss")
 @click.option(
     "--request",
     type=str,
     required=False,
     help="String formatted as json that represents request",
 )
```

### Comparing `truss-0.4.8rc8/truss/constants.py` & `truss-0.4.9rc2/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/image_builder/image_builder.py` & `truss-0.4.9rc2/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.9rc2/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.9rc2/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/image_builder/util.py` & `truss-0.4.9rc2/truss/contexts/image_builder/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # manual nature is by design; at this point we want any new base image releases
 # to be reviewed via code change before landing. This value should be typically
 # set to the latest version of truss library.
 #
 # [IMPORTANT] Make sure all images for this version are published to dockerhub
 # before change to this value lands. This value is used to look for base images
 # when building docker image for a truss.
-TRUSS_BASE_IMAGE_VERSION_TAG = "v0.4.8"
+TRUSS_BASE_IMAGE_VERSION_TAG = "v0.4.9"
 
 
 def file_is_empty(path: Path, ignore_hash_style_comments: bool = True) -> bool:
     if not path.exists():
         return True
 
     with path.open() as file:
```

### Comparing `truss-0.4.8rc8/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.4.9rc2/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.9rc2/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/local_loader/train_local.py` & `truss-0.4.9rc2/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.9rc2/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/contexts/local_loader/utils.py` & `truss-0.4.9rc2/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/docker.py` & `truss-0.4.9rc2/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/environment_inference/requirements_inference.py` & `truss-0.4.9rc2/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/errors.py` & `truss-0.4.9rc2/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/local/local_config.py` & `truss-0.4.9rc2/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/local/local_config_handler.py` & `truss-0.4.9rc2/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_framework.py` & `truss-0.4.9rc2/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/__init__.py` & `truss-0.4.9rc2/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.9rc2/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/keras.py` & `truss-0.4.9rc2/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/lightgbm.py` & `truss-0.4.9rc2/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/mlflow.py` & `truss-0.4.9rc2/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/pytorch.py` & `truss-0.4.9rc2/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/sklearn.py` & `truss-0.4.9rc2/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_frameworks/xgboost.py` & `truss-0.4.9rc2/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/model_inference.py` & `truss-0.4.9rc2/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/patch/calc_patch.py` & `truss-0.4.9rc2/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/patch/dir_signature.py` & `truss-0.4.9rc2/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/patch/hash.py` & `truss-0.4.9rc2/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/patch/types.py` & `truss-0.4.9rc2/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/readme_generator.py` & `truss-0.4.9rc2/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/README.md.jinja` & `truss-0.4.9rc2/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/base.Dockerfile.jinja` & `truss-0.4.9rc2/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/control/control/endpoints.py` & `truss-0.4.9rc2/truss/templates/control/control/endpoints.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 from typing import Any, Dict
 
 import requests
-from flask import Blueprint, Response, current_app, jsonify, request
-from helpers.errors import ModelNotReady
+from fastapi import APIRouter, Request, Response
+from fastapi.responses import JSONResponse
+from helpers.errors import ModelLoadFailed, ModelNotReady
 from requests.exceptions import ConnectionError
 from tenacity import Retrying, retry_if_exception_type, stop_after_attempt, wait_fixed
 
 INFERENCE_SERVER_START_WAIT_SECS = 60
 
 
-control_app = Blueprint("control", __name__)
+control_app = APIRouter()
 
 
-@control_app.route("/")
+@control_app.get("/")
 def index():
-    return jsonify({})
+    return {}
 
 
-@control_app.route("/v1/<path:path>", methods=["GET", "POST"])
-def proxy(path):
-    inference_server_port = current_app.config["inference_server_port"]
-    inference_server_process_controller = current_app.config[
-        "inference_server_process_controller"
-    ]
+@control_app.get("/v1/{full_path:path}")
+@control_app.post("/v1/{full_path:path}")
+async def proxy(full_path: str, request: Request):
+    inference_server_port = request.app.state.inference_server_port
+    inference_server_process_controller = (
+        request.app.state.inference_server_process_controller
+    )
 
     # Wait a bit for inference server to start
     for attempt in Retrying(
         retry=(
             retry_if_exception_type(ConnectionError)
             | retry_if_exception_type(ModelNotReady)
         ),
         stop=stop_after_attempt(INFERENCE_SERVER_START_WAIT_SECS),
         wait=wait_fixed(1),
     ):
         with attempt:
             try:
+                if (
+                    inference_server_process_controller.is_inference_server_intentionally_stopped()
+                ):
+                    raise ModelLoadFailed("Model load failed")
+
                 resp = requests.request(
                     method=request.method,
-                    url=f"http://localhost:{inference_server_port}/v1/{path}",
-                    data=request.get_data(),
+                    url=f"http://localhost:{inference_server_port}/v1/{full_path}",
+                    data=await request.body(),
                     cookies=request.cookies,
                     headers=request.headers,
                 )
                 if _is_model_not_ready(resp):
                     raise ModelNotReady("Model has started running, but not ready yet.")
             except ConnectionError as exp:
                 # This check is a bit expensive so we don't do it before every request, we
@@ -51,55 +58,54 @@
                 # otherwise we bail.
                 if (
                     inference_server_process_controller.inference_server_ever_started()
                     and not inference_server_process_controller.is_inference_server_running()
                 ):
                     error_msg = "It appears your model has stopped running. This often means' \
                         ' it crashed and may need a fix to get it running again."
-                    return Response(error_msg, 503)
+                    return JSONResponse(error_msg, 503)
                 raise exp
 
-    headers = [(name, value) for (name, value) in resp.raw.headers.items()]
-    response = Response(resp.content, resp.status_code, headers)
+    response = Response(resp.content, resp.status_code, resp.headers)
     return response
 
 
-@control_app.route("/control/patch", methods=["POST"])
-def patch() -> Dict[str, str]:
-    current_app.logger.info("Patch request received.")
-    patch_request = request.get_json()
-    current_app.config["inference_server_controller"].apply_patch(patch_request)
-    current_app.logger.info("Patch applied successfully")
+@control_app.post("/control/patch")
+async def patch(request: Request) -> Dict[str, str]:
+    request.app.state.logger.info("Patch request received.")
+    patch_request = await request.json()
+    request.app.state.inference_server_controller.apply_patch(patch_request)
+    request.app.state.logger.info("Patch applied successfully")
     return {"msg": "Patch applied successfully"}
 
 
-@control_app.route("/control/truss_hash", methods=["GET"])
-def truss_hash() -> Dict[str, Any]:
-    t_hash = current_app.config["inference_server_controller"].truss_hash()
+@control_app.get("/control/truss_hash")
+def truss_hash(request: Request) -> Dict[str, Any]:
+    t_hash = request.app.state.inference_server_controller.truss_hash()
     return {"result": t_hash}
 
 
-@control_app.route("/control/restart_inference_server", methods=["POST"])
-def restart_inference_server() -> Dict[str, str]:
-    current_app.config["inference_server_controller"].restart()
+@control_app.post("/control/restart_inference_server")
+def restart_inference_server(request: Request) -> Dict[str, str]:
+    request.app.state.inference_server_controller.restart()
 
     return {"msg": "Inference server started successfully"}
 
 
-@control_app.route("/control/has_partially_applied_patch", methods=["GET"])
-def has_partially_applied_patch() -> Dict[str, Any]:
-    app_has_partially_applied_patch = current_app.config[
-        "inference_server_controller"
-    ].has_partially_applied_patch()
+@control_app.get("/control/has_partially_applied_patch")
+def has_partially_applied_patch(request: Request) -> Dict[str, Any]:
+    app_has_partially_applied_patch = (
+        request.app.state.inference_server_controller.has_partially_applied_patch()
+    )
     return {"result": app_has_partially_applied_patch}
 
 
-@control_app.route("/control/stop_inference_server", methods=["POST"])
-def stop_inference_server() -> Dict[str, str]:
-    current_app.config["inference_server_controller"].stop()
+@control_app.post("/control/stop_inference_server")
+def stop_inference_server(request: Request) -> Dict[str, str]:
+    request.app.state.inference_server_controller.stop()
     return {"msg": "Inference server stopped successfully"}
 
 
 def _is_model_not_ready(resp) -> bool:
     return (
         resp.status_code == 503
         and resp.content is not None
```

### Comparing `truss-0.4.8rc8/truss/templates/control/control/helpers/errors.py` & `truss-0.4.9rc2/truss/templates/control/control/helpers/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,7 +36,13 @@
     pass
 
 
 class ModelNotReady(Error):
     """Model has started running, but not ready yet."""
 
     pass
+
+
+class ModelLoadFailed(Error):
+    """Model has failed to load."""
+
+    pass
```

### Comparing `truss-0.4.8rc8/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 import os
 import signal
 import subprocess
+from pathlib import Path
 from typing import List, Optional
 
 from helpers.context_managers import current_directory
 
+INFERENCE_SERVER_FAILED_FILE = Path("~/inference_server_crashed.txt").expanduser()
 
-class InferenceServerProcessController:
 
+class InferenceServerProcessController:
     _inference_server_process: Optional[subprocess.Popen] = None
     _inference_server_port: int
     _inference_server_home: str
     _app_logger: logging.Logger
     _inference_server_process_args: List[str]
 
     def __init__(
@@ -63,13 +65,19 @@
             return False
 
         if self._inference_server_process is None:
             return False
 
         return self._inference_server_process.poll() is None
 
+    def is_inference_server_intentionally_stopped(self) -> bool:
+        return INFERENCE_SERVER_FAILED_FILE.exists()
+
     def check_and_recover_inference_server(self):
         if self.inference_server_started() and not self.is_inference_server_running():
-            self._app_logger.warning(
-                "Inference server seems to have crashed, restarting"
-            )
-            self.start()
+            if not self.is_inference_server_intentionally_stopped():
+                self._app_logger.warning(
+                    "Inference server seems to have crashed, restarting"
+                )
+                self.start()
+            else:
+                self._app_logger.warning("Inference server unrecoverable. Try patching")
```

### Comparing `truss-0.4.8rc8/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 import requests
+from fastapi import FastAPI
 from tenacity import Retrying, stop_after_attempt, wait_exponential
 
 
-def inference_server_startup_flow(application) -> None:
+def inference_server_startup_flow(application: FastAPI) -> None:
     """
     Perform the inference server startup flow
 
     Inference server startup flow supports checking for patches. If a patch ping
     url is provided then we hit that url to start the sync mechanism. The ping
     calls with current truss hash. The patch ping endpoint should return a
     response indicating, either that the supplied hash is current or that the
@@ -20,41 +21,41 @@
 
     The goal is to start the inference server as soon as we have the latest
     code, but not before.
     Example responses:
     {"is_current": true}
     {"accepted": true}
     """
-    inference_server_controller = application.config["inference_server_controller"]
+    inference_server_controller = application.state.inference_server_controller
     patch_ping_url = os.environ.get("PATCH_PING_URL_TRUSS")
     if patch_ping_url is None:
         inference_server_controller.start()
         return
 
     truss_hash = inference_server_controller.truss_hash()
     payload = {"truss_hash": truss_hash}
 
     for attempt in Retrying(
         stop=stop_after_attempt(15),
         wait=wait_exponential(multiplier=2, min=1, max=4),
     ):
         with attempt:
             try:
-                application.logger.info(
+                application.state.logger.info(
                     f"Pinging {patch_ping_url} for patch with hash {truss_hash}"
                 )
                 resp = requests.post(patch_ping_url, json=payload)
                 resp.raise_for_status()
                 resp_body = resp.json()
 
                 # If hash is current start inference server, otherwise delay that
                 # for when patch is applied.
                 if "is_current" in resp_body and resp_body["is_current"] is True:
-                    application.logger.info(
+                    application.state.logger.info(
                         "Hash is current, starting inference server"
                     )
                     inference_server_controller.start()
             except Exception as exc:  # noqa
-                application.logger.warning(
+                application.state.logger.warning(
                     f"Patch ping attempt failed with error {exc}"
                 )
                 raise exc
```

### Comparing `truss-0.4.8rc8/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.9rc2/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/control/control/helpers/types.py` & `truss-0.4.9rc2/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/control/control/server.py` & `truss-0.4.9rc2/truss/templates/control/control/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 from pathlib import Path
 from threading import Thread
-from typing import Union
 
 from application import create_app
 from helpers.inference_server_starter import inference_server_startup_flow
-from waitress.server import BaseWSGIServer, MultiSocketServer
 
 CONTROL_SERVER_PORT = int(os.environ.get("CONTROL_SERVER_PORT", "8080"))
 INFERENCE_SERVER_PORT = int(os.environ.get("INFERENCE_SERVER_PORT", "8090"))
 PYTHON_EXECUTABLE_LOOKUP_PATHS = [
     "/usr/local/bin/python",
     "/usr/local/bin/python3",
     "/usr/bin/python",
@@ -22,15 +20,15 @@
         if Path(path).exists():
             return path
 
     raise RuntimeError("Unable to find python, make sure it's installed.")
 
 
 if __name__ == "__main__":
-    from waitress import create_server
+    import uvicorn
 
     inf_serv_home: str = os.environ["APP_HOME"]
     python_executable_path: str = _identify_python_executable_path()
     application = create_app(
         {
             "inference_server_home": inf_serv_home,
             "inference_server_process_args": [
@@ -42,16 +40,21 @@
             "inference_server_port": INFERENCE_SERVER_PORT,
         }
     )
 
     # Perform inference server startup flow in background
     Thread(target=inference_server_startup_flow, args=(application,)).start()
 
-    application.logger.info(
+    application.state.logger.info(
         f"Starting live reload server on port {CONTROL_SERVER_PORT}"
     )
-    server: Union[BaseWSGIServer, MultiSocketServer] = create_server(
+    uvicorn.run(
         application,
-        host=application.config["control_server_host"],
-        port=application.config["control_server_port"],
+        host=application.state.control_server_host,
+        port=application.state.control_server_port,
+        loop="uvloop",
+        reload=False,
+        # TODO(pankaj): change this back to info once things are stable
+        log_level="debug",
+        workers=1,
+        limit_concurrency=32,
     )
-    server.run()
```

### Comparing `truss-0.4.8rc8/truss/templates/custom/model/model.py` & `truss-0.4.9rc2/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.9rc2/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/keras/model/model.py` & `truss-0.4.9rc2/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/lightgbm/model/model.py` & `truss-0.4.9rc2/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/mlflow/model/model.py` & `truss-0.4.9rc2/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/pytorch/model/model.py` & `truss-0.4.9rc2/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/common/errors.py` & `truss-0.4.9rc2/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/common/logging.py` & `truss-0.4.9rc2/truss/templates/control/control/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.4.9rc2/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/common/patches.py` & `truss-0.4.9rc2/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/common/retry.py` & `truss-0.4.9rc2/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/common/serialization.py` & `truss-0.4.9rc2/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/common/truss_server.py` & `truss-0.4.9rc2/truss/templates/server/common/truss_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import asyncio
 import concurrent.futures
 import json
 import logging
 import multiprocessing
+import os
+import signal
 import socket
+from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 import common.errors as errors
 import common.util as utils
 import uvicorn
 from common.logging import setup_logging
 from common.serialization import (
@@ -27,14 +30,15 @@
     Used by FastAPI to read body in an asynchronous manner
     """
     return await request.body()
 
 
 FORMAT = "%(asctime)s.%(msecs)03d %(name)s %(levelname)s [%(funcName)s():%(lineno)s] %(message)s"
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
+INFERENCE_SERVER_FAILED_FILE = Path("~/inference_server_crashed.txt").expanduser()
 logging.basicConfig(level=logging.INFO, format=FORMAT, datefmt=DATE_FORMAT)
 
 
 class UvicornCustomServer(multiprocessing.Process):
     def __init__(
         self, config: uvicorn.Config, sockets: Optional[List[socket.socket]] = None
     ):
@@ -65,15 +69,16 @@
         if model_name != self._model.name:
             raise errors.ModelMissingError(model_name)
         return self._model
 
     @staticmethod
     def check_healthy(model: ModelWrapper):
         if model.load_failed():
-            raise errors.InferenceError("Model load failed")
+            INFERENCE_SERVER_FAILED_FILE.touch()
+            os.kill(os.getpid(), signal.SIGKILL)
 
         if not model.ready:
             raise errors.ModelNotReady(model.name)
 
     async def model_ready(self, model_name: str) -> Dict[str, Union[str, bool]]:
         self.check_healthy(self._safe_lookup_model(model_name))
 
@@ -134,25 +139,38 @@
         return (
             "Content-Type" in request.headers
             and request.headers["Content-Type"] == "application/octet-stream"
         )
 
 
 class TrussServer:
-    def __init__(self, http_port: int, config: Dict):
+    def __init__(
+        self,
+        http_port: int,
+        config: Dict,
+        setup_json_logger: bool = True,
+    ):
         self.http_port = http_port
         self._config = config
         self._model = ModelWrapper(self._config)
         self._endpoints = BasetenEndpoints(self._model)
+        self._setup_json_logger = setup_json_logger
+
+    def cleanup(self):
+        if INFERENCE_SERVER_FAILED_FILE.exists():
+            INFERENCE_SERVER_FAILED_FILE.unlink()
 
     def on_startup(self):
         """
         This method will be started inside the main process, so here is where we want to setup our logging and model
         """
-        setup_logging()
+        self.cleanup()
+
+        if self._setup_json_logger:
+            setup_logging()
 
         self._model.start_load()
 
     def create_application(self):
         return FastAPI(
             title="Baseten Inference Server",
             docs_url=None,
@@ -240,14 +258,16 @@
                     },
                 },
             },
         )
 
         max_asyncio_workers = min(32, utils.cpu_count() + 4)
         logging.info(f"Setting max asyncio worker threads as {max_asyncio_workers}")
+        # Call this so uvloop gets used
+        cfg.setup_event_loop()
         asyncio.get_event_loop().set_default_executor(
             concurrent.futures.ThreadPoolExecutor(max_workers=max_asyncio_workers)
         )
 
         async def serve():
             serversocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             serversocket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
```

### Comparing `truss-0.4.8rc8/truss/templates/server/common/util.py` & `truss-0.4.9rc2/truss/templates/server/common/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/inference_server.py` & `truss-0.4.9rc2/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server/model_wrapper.py` & `truss-0.4.9rc2/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/server.Dockerfile.jinja` & `truss-0.4.9rc2/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/shared/secrets_resolver.py` & `truss-0.4.9rc2/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/sklearn/model/model.py` & `truss-0.4.9rc2/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/training/job.py` & `truss-0.4.9rc2/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/templates/xgboost/model/model.py` & `truss-0.4.9rc2/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/auto-mpg.data` & `truss-0.4.9rc2/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/happy.ipynb` & `truss-0.4.9rc2/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.9rc2/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.9rc2/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/readme_int_example.md` & `truss-0.4.9rc2/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/readme_no_example.md` & `truss-0.4.9rc2/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/readme_str_example.md` & `truss-0.4.9rc2/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/server.Dockerfile` & `truss-0.4.9rc2/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/test_truss/config.yaml` & `truss-0.4.9rc2/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/test_data/test_truss/model/model.py` & `truss-0.4.9rc2/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/conftest.py` & `truss-0.4.9rc2/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.4.9rc2/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.9rc2/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.9rc2/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.9rc2/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/local/test_local_config_handler.py` & `truss-0.4.9rc2/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.9rc2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.9rc2/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.9rc2/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.9rc2/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.9rc2/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.9rc2/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/patch/test_calc_patch.py` & `truss-0.4.9rc2/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/patch/test_hash.py` & `truss-0.4.9rc2/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/samples.py` & `truss-0.4.9rc2/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.9rc2/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/templates/control/control/test_server.py` & `truss-0.4.9rc2/truss/tests/templates/control/control/test_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, List
 
 import pytest
+from fastapi.testclient import TestClient
 
 # Needed to simulate the set up on the model docker container
 sys.path.append(
     str(
         Path(__file__).parent.parent.parent.parent.parent
         / "templates"
         / "control"
@@ -42,38 +43,38 @@
                 "control_server_host": "*",
                 "control_server_port": 8081,
                 "inference_server_port": 8082,
                 "oversee_inference_server": False,
                 "pip_path": "pip",
             }
         )
-        inference_server_controller = control_app.config["inference_server_controller"]
+        inference_server_controller = control_app.state.inference_server_controller
         try:
             inference_server_controller.start()
             yield control_app
         finally:
             inference_server_controller.stop()
 
 
 @pytest.fixture()
 def client(app):
-    return app.test_client()
+    return TestClient(app)
 
 
 def test_restart_server(client):
     resp = client.post("/control/stop_inference_server")
     assert resp.status_code == 200
-    assert "error" not in resp.json
-    assert "msg" in resp.json
+    assert "error" not in resp.json()
+    assert "msg" in resp.json()
 
     # Try second restart
     resp = client.post("/control/stop_inference_server")
     assert resp.status_code == 200
-    assert "error" not in resp.json
-    assert "msg" in resp.json
+    assert "error" not in resp.json()
+    assert "msg" in resp.json()
 
 
 def test_patch_model_code_update_existing(app, client):
     mock_model_file_content = """
 class Model:
     def predict(self, request):
         return {'prediction': [1]}
@@ -83,17 +84,15 @@
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="model.py",
             content=mock_model_file_content,
         ),
     )
     _verify_apply_patch_success(client, patch)
-    with (
-        app.config["inference_server_home"] / "model" / "model.py"
-    ).open() as model_file:
+    with (app.state.inference_server_home / "model" / "model.py").open() as model_file:
         new_model_file_content = model_file.read()
     assert new_model_file_content == mock_model_file_content
 
 
 def test_patch_model_code_update_predict_on_long_load_time(app, client):
     mock_model_file_content = """
 class Model:
@@ -111,44 +110,44 @@
             path="model.py",
             content=mock_model_file_content,
         ),
     )
     _verify_apply_patch_success(client, patch)
     resp = client.post("/v1/models/model:predict", json={})
     resp.status_code == 200
-    assert resp.json == {"prediction": [1]}
+    assert resp.json() == {"prediction": [1]}
 
 
 def test_patch_model_code_create_new(app, client):
     empty_content = ""
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="touched",
             content=empty_content,
         ),
     )
     _verify_apply_patch_success(client, patch)
-    assert (app.config["inference_server_home"] / "model" / "touched").exists()
+    assert (app.state.inference_server_home / "model" / "touched").exists()
 
 
 def test_patch_model_code_create_in_new_dir(app, client):
     empty_content = ""
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="new_directory/touched",
             content=empty_content,
         ),
     )
     _verify_apply_patch_success(client, patch)
     assert (
-        app.config["inference_server_home"] / "model" / "new_directory" / "touched"
+        app.state.inference_server_home / "model" / "new_directory" / "touched"
     ).exists()
 
 
 def test_404(client):
     resp = client.post("/control/nonexitant")
     assert resp.status_code == 404
 
@@ -157,41 +156,41 @@
     patch_request = {
         "hash": "dummy",
         "prev_hash": "invalid",
         "patches": [],
     }
     resp = client.post("/control/patch", json=patch_request)
     assert resp.status_code == 200
-    assert "error" in resp.json
-    assert resp.json["error"]["type"] == "inadmissible_patch"
-    assert "msg" not in resp.json
+    assert "error" in resp.json()
+    assert resp.json()["error"]["type"] == "inadmissible_patch"
+    assert "msg" not in resp.json()
 
 
 def test_unsupported_patch(client):
     unsupported_patch = {
         "type": "unsupported",
         "body": {},
     }
     resp = _apply_patches(client, [unsupported_patch])
     assert resp.status_code == 200
-    assert "error" in resp.json
-    assert resp.json["error"]["type"] == "unsupported_patch"
+    assert "error" in resp.json()
+    assert resp.json()["error"]["type"] == "unsupported_patch"
 
 
 def test_patch_failed_recoverable(client):
     will_fail_patch = Patch(
         type=PatchType.PYTHON_REQUIREMENT,
         body=PythonRequirementPatch(
             action=Action.ADD, requirement="not_a_valid_python_requirement"
         ),
     )
     resp = _apply_patches(client, [will_fail_patch.to_dict()])
     assert resp.status_code == 200
-    assert "error" in resp.json
-    assert resp.json["error"]["type"] == "patch_failed_recoverable"
+    assert "error" in resp.json()
+    assert resp.json()["error"]["type"] == "patch_failed_recoverable"
 
 
 def test_patch_failed_unrecoverable(client):
     will_pass_patch = Patch(
         type=PatchType.PYTHON_REQUIREMENT,
         body=PythonRequirementPatch(action=Action.ADD, requirement="requests"),
     )
@@ -201,34 +200,34 @@
             action=Action.ADD, requirement="not_a_valid_python_requirement"
         ),
     )
     resp = _apply_patches(
         client, [will_pass_patch.to_dict(), will_fail_patch.to_dict()]
     )
     assert resp.status_code == 200
-    assert "error" in resp.json
-    assert resp.json["error"]["type"] == "patch_failed_unrecoverable"
+    assert "error" in resp.json()
+    assert resp.json()["error"]["type"] == "patch_failed_unrecoverable"
 
 
 def _verify_apply_patch_success(client, patch: Patch):
-    original_hash = client.get("/control/truss_hash").json["result"]
+    original_hash = client.get("/control/truss_hash").json()["result"]
     patch_request = {
         "hash": "dummy",
         "prev_hash": original_hash,
         "patches": [patch.to_dict()],
     }
     resp = client.post("/control/patch", json=patch_request)
     resp = _apply_patches(client, [patch.to_dict()])
     assert resp.status_code == 200
-    assert "error" not in resp.json
-    assert "msg" in resp.json
+    assert "error" not in resp.json()
+    assert "msg" in resp.json()
 
 
 def _apply_patches(client, patches: List[dict]):
-    original_hash = client.get("/control/truss_hash").json["result"]
+    original_hash = client.get("/control/truss_hash").json()["result"]
     patch_request = {
         "hash": "dummy",
         "prev_hash": original_hash,
         "patches": patches,
     }
     return client.post("/control/patch", json=patch_request)
```

### Comparing `truss-0.4.8rc8/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.9rc2/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.9rc2/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/templates/server/common/test_retry.py` & `truss-0.4.9rc2/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.4.9rc2/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_backward.py` & `truss-0.4.9rc2/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_build.py` & `truss-0.4.9rc2/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_config.py` & `truss-0.4.9rc2/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_context_builder_image.py` & `truss-0.4.9rc2/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_docker.py` & `truss-0.4.9rc2/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_notebooks.py` & `truss-0.4.9rc2/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.9rc2/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_truss_gatherer.py` & `truss-0.4.9rc2/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/tests/test_truss_handle.py` & `truss-0.4.9rc2/truss/tests/test_truss_handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 import pytest
 import requests
 from python_on_whales.exceptions import DockerException
+from tenacity import RetryError
 from truss.docker import Docker, DockerStates
 from truss.errors import ContainerIsDownError, ContainerNotFoundError
 from truss.local.local_config_handler import LocalConfigHandler
 from truss.templates.control.control.helpers.types import (
     Action,
     ModelCodePatch,
     Patch,
@@ -832,18 +833,18 @@
         bad_model_code = """
 class Model:
     def malformed
 """
         model_code_file_path = custom_model_control / "model" / "model.py"
         with model_code_file_path.open("w") as model_code_file:
             model_code_file.write(bad_model_code)
-        with pytest.raises(requests.exceptions.HTTPError) as exc_info:
+        with pytest.raises(RetryError) as exc_info:
             th.docker_predict([1], tag=tag)
-        resp = exc_info.value.response
-        assert resp.status_code == 500
+        resp = exc_info.value.last_attempt.result()
+        assert resp.status_code == 503
         assert "Model load failed" in resp.text
 
         # Should be able to fix code after
         good_model_code = """
 class Model:
     def predict(self, model_input):
         return [2 for i in model_input]
```

### Comparing `truss-0.4.8rc8/truss/tests/test_validation.py` & `truss-0.4.9rc2/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/truss_config.py` & `truss-0.4.9rc2/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/truss_gatherer.py` & `truss-0.4.9rc2/truss/truss_gatherer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from pathlib import Path
 
 import yaml
 from truss.local.local_config_handler import LocalConfigHandler
-from truss.patch.hash import str_hash_str
 from truss.truss_handle import TrussHandle
-from truss.util.path import copy_file_path, copy_tree_path, remove_tree_path
+from truss.util.path import (
+    calc_shadow_truss_dirname,
+    copy_file_path,
+    copy_tree_path,
+    remove_tree_path,
+)
 
 
 def gather(truss_path: Path) -> Path:
     handle = TrussHandle(truss_path)
-    shadow_truss_dir_name = _calc_shadow_truss_dirname(truss_path)
+    shadow_truss_dir_name = calc_shadow_truss_dirname(truss_path)
     shadow_truss_metdata_file_path = (
         LocalConfigHandler.shadow_trusses_dir_path()
         / f"{shadow_truss_dir_name}.metadata.yaml"
     )
     shadow_truss_path = (
         LocalConfigHandler.shadow_trusses_dir_path() / shadow_truss_dir_name
     )
@@ -56,12 +60,7 @@
     # packages. We do it after.
     shadow_handle = TrussHandle(shadow_truss_path, validate=False)
     shadow_handle.clear_external_packages()
     shadow_handle.validate()
     with shadow_truss_metdata_file_path.open("w") as fp:
         yaml.safe_dump({"max_mod_time": handle.max_modified_time}, fp)
     return shadow_truss_path
-
-
-def _calc_shadow_truss_dirname(truss_path: Path) -> str:
-    resolved_path_str = str(truss_path.resolve())
-    return str_hash_str(resolved_path_str)
```

### Comparing `truss-0.4.8rc8/truss/truss_handle.py` & `truss-0.4.9rc2/truss/truss_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from truss.contexts.image_builder.serving_image_builder import (
     ServingImageBuilderContext,
 )
 from truss.contexts.image_builder.training_image_builder import (
     TrainingImageBuilderContext,
 )
 from truss.contexts.local_loader.load_model_local import LoadModelLocal
+from truss.contexts.local_loader.local_server_loader import LocalServerLoader
 from truss.contexts.local_loader.train_local import LocalTrainer
 from truss.decorators import proxy_to_shadow_if_scattered
 from truss.docker import (
     Docker,
     DockerStates,
     get_container_logs,
     get_container_state,
@@ -384,14 +385,24 @@
         Returns:
             docker build command.
         """
         image_builder = ServingImageBuilderContext.run(self._truss_dir)
         image_builder.prepare_image_build_dir(build_dir)
         return image_builder.docker_build_command(build_dir)
 
+    def run_local_server_with_reload(
+        self,
+        build_dir: Optional[Path] = None,
+        work_dir: Optional[Path] = None,
+        port: Optional[int] = None,
+    ):
+        image_builder = ServingImageBuilderContext.run(self._truss_dir)
+        server_loader = LocalServerLoader(self._truss_dir, image_builder, port=port)
+        server_loader.watch(build_dir, work_dir)
+
     @proxy_to_shadow_if_scattered
     def training_docker_build_setup(self, build_dir: Optional[Path] = None):
         """
         Set up a directory to build training docker image from.
 
         Returns:
             docker build command.
```

### Comparing `truss-0.4.8rc8/truss/truss_spec.py` & `truss-0.4.9rc2/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/types.py` & `truss-0.4.9rc2/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/util/gpu.py` & `truss-0.4.9rc2/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/truss/util/path.py` & `truss-0.4.9rc2/truss/util/path.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 import tempfile
 from contextlib import contextmanager
 from distutils.dir_util import copy_tree, remove_tree
 from distutils.file_util import copy_file
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
+from truss.patch.hash import str_hash_str
+
 
 def copy_tree_path(src: Path, dest: Path) -> List[str]:
-    return copy_tree(str(src), str(dest))
+    return copy_tree(str(src), str(dest), verbose=0)
 
 
 def copy_file_path(src: Path, dest: Path) -> Tuple[str, str]:
-    return copy_file(str(src), str(dest))
+    return copy_file(str(src), str(dest), verbose=False)
 
 
 def copy_tree_or_file(src: Path, dest: Path) -> Union[List[str], Tuple[str, str]]:
     if src.is_file():
         return copy_file_path(src, dest)
 
     return copy_tree_path(src, dest)
 
 
 def remove_tree_path(target: Path) -> None:
-    return remove_tree(str(target))
+    return remove_tree(str(target), verbose=0)
 
 
 def get_max_modified_time_of_dir(path: Path) -> float:
     max_modified_time = os.path.getmtime(path)
     for root, dirs, files in os.walk(path):
         if os.path.islink(root):
             raise ValueError(f"Symlinks not allowed in Truss: {root}")
@@ -56,7 +58,20 @@
     """Builds a directory under ~/.truss/models for the purpose of creating a Truss at."""
     rand_suffix = "".join(random.choices(string.ascii_uppercase + string.digits, k=6))
     target_directory_path = Path(
         Path.home(), ".truss", "models", f"{stub}-{rand_suffix}"
     )
     target_directory_path.mkdir(parents=True)
     return target_directory_path
+
+
+def calc_shadow_truss_dirname(truss_path: Path) -> str:
+    resolved_path_str = str(truss_path.resolve())
+    return str_hash_str(resolved_path_str)
+
+
+def build_truss_shadow_target_directory(stub: str, truss_path: Path) -> Path:
+    """Builds a directory under ~/.truss/models."""
+    suffix = calc_shadow_truss_dirname(truss_path)
+    target_directory_path = Path(Path.home(), ".truss", "models", f"{stub}-{suffix}")
+    target_directory_path.mkdir(parents=True, exist_ok=True)
+    return target_directory_path
```

### Comparing `truss-0.4.8rc8/truss/validation.py` & `truss-0.4.9rc2/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc8/PKG-INFO` & `truss-0.4.9rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.8rc8
+Version: 0.4.9rc2
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
@@ -27,14 +27,17 @@
 Requires-Dist: packaging (>=20.9,<21.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: python-json-logger (>=2.0.2)
 Requires-Dist: python-on-whales (>=0.46.0,<0.47.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
+Requires-Dist: virtualenv (>=20.23.0,<21.0.0)
+Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
+Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Project-URL: Bug Reports, https://github.com/basetenlabs/truss/issues
 Project-URL: Baseten, https://baseten.co
 Project-URL: Documentation, https://truss.baseten.co
 Project-URL: Homepage, https://truss.baseten.co
 Project-URL: Repository, https://github.com/basetenlabs/truss
 Description-Content-Type: text/markdown
```

