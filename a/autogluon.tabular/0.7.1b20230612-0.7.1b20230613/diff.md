# Comparing `tmp/autogluon.tabular-0.7.1b20230612.tar.gz` & `tmp/autogluon.tabular-0.7.1b20230613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.7.1b20230612.tar", last modified: Mon Jun 12 09:04:07 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.7.1b20230613.tar", last modified: Tue Jun 13 09:04:13 2023, max compression
```

## Comparing `autogluon.tabular-0.7.1b20230612.tar` & `autogluon.tabular-0.7.1b20230613.tar`

### file list

```diff
@@ -1,170 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.947244 autogluon.tabular-0.7.1b20230612/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.947244 autogluon.tabular-0.7.1b20230612/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.955245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.955245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.955245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48580 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.955245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.955245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.959245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.963245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.967245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)   251990 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.971245 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-12 09:03:34.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:04:07.955245 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:04:07.000000 autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.606497 autogluon.tabular-0.7.1b20230613/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.606497 autogluon.tabular-0.7.1b20230613/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   266100 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.7.1b20230612/PKG-INFO` & `autogluon.tabular-0.7.1b20230613/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230612
+Version: 0.7.1b20230613
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -178,14 +178,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: lightgbm
 Provides-Extra: catboost
 Provides-Extra: xgboost
 Provides-Extra: fastai
+Provides-Extra: tabpfn
 Provides-Extra: ray
 Provides-Extra: skex
 Provides-Extra: imodels
 Provides-Extra: vowpalwabbit
 Provides-Extra: skl2onnx
 Provides-Extra: all
 Provides-Extra: tests
```

### Comparing `autogluon.tabular-0.7.1b20230612/setup.py` & `autogluon.tabular-0.7.1b20230613/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     'xgboost': [
         'xgboost>=1.6,<1.8',
     ],
     'fastai': [
         'torch>=1.9,<1.14',
         'fastai>=2.3.1,<2.8',
     ],
+    'tabpfn': [
+        'tabpfn>=0.1,<0.2',
+    ],
     'ray': [
         f'{ag.PACKAGE_NAME}.core[all]=={version}',
     ],
     'skex': [
         # Note: 2021.7 released on Sep 2022, version 2022.x doesn't exist (went directly from 2021.7 to 2023.0)
         'scikit-learn-intelex>=2021.7,<2023.2',
     ],
@@ -70,24 +73,25 @@
         'onnxruntime>=1.13.0,<1.14.0'
     ] if sys.platform == 'darwin' else [
         'skl2onnx>=1.13.0,<1.14.0',
         'onnxruntime-gpu>=1.13.0,<1.14.0'
     ]
 }
 
+# TODO: v1.0: Rename `all` to `core`, make `all` contain everything.
 all_requires = []
 # TODO: Consider adding 'skex' to 'all'
 for extra_package in ['lightgbm', 'catboost', 'xgboost', 'fastai', 'ray']:
     all_requires += extras_require[extra_package]
 all_requires = list(set(all_requires))
 extras_require['all'] = all_requires
 
 
 test_requires = []
-for test_package in ['imodels', 'vowpalwabbit', 'skl2onnx']:
+for test_package in ['tabpfn', 'imodels', 'vowpalwabbit', 'skl2onnx']:
     test_requires += extras_require[test_package]
 extras_require['tests'] = test_requires
 install_requires = ag.get_dependency_version_ranges(install_requires)
 
 if __name__ == '__main__':
     ag.create_version_file(version=version, submodule=submodule)
     setup_args = ag.default_setup_args(version=version, submodule=submodule)
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,18 @@
     }
 )
 
 # default_FTT is experimental
 hyperparameter_config_dict['default_FTT'] = {'FT_TRANSFORMER': {}}
 hyperparameter_config_dict['default_FTT'].update(hyperparameter_config_dict['default'])
 
+# extreme is experimental
+hyperparameter_config_dict['extreme'] = {'TABPFN': {'N_ensemble_configurations': 8}}
+hyperparameter_config_dict['extreme'].update(hyperparameter_config_dict['default_FTT'])
+
 
 def get_hyperparameter_config_options():
     return list(hyperparameter_config_dict.keys())
 
 
 def get_hyperparameter_config(config_name):
     config_options = get_hyperparameter_config_options()
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/presets_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     # ------------------------------------------
     # Experimental presets. Only use these presets if you are ok with unstable and potentially poor performing presets.
     #  Experimental presets can be removed or changed without warning.
 
     # Best quality with an additional FTTransformer model, GPU is recommended.
     experimental_best_quality={'auto_stack': True, 'hyperparameters': 'default_FTT'},
 
+    # Best quality with an additional FTTransformer and TabPFN model, GPU is recommended.
+    #  May have **extremely** slow inference speed, to a potentially unusable degree.
+    experimental_extreme_quality={'auto_stack': True, 'hyperparameters': 'extreme'},
+
     # ------------------------------------------
     # ------------------------------------------
     # ------------------------------------------
 
     # TODO: Consider HPO-enabled configs if training time doesn't matter but inference latency does.
 )
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from __future__ import annotations
+
 import copy
 import json
 import logging
 import time
 from collections.abc import Iterable
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
-from typing import List
+from typing import List, Union
 from sklearn.metrics import classification_report
 
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, AUTO_WEIGHT, BALANCE_WEIGHT
 from autogluon.core.data.label_cleaner import LabelCleaner, LabelCleanerMulticlassToBinary
 from autogluon.core.learner import AbstractLearner
-from autogluon.core.metrics import confusion_matrix, get_metric
+from autogluon.core.metrics import confusion_matrix, get_metric, Scorer
 from autogluon.core.models.greedy_ensemble.ensemble_selection import EnsembleSelection
 from autogluon.core.utils import get_leaderboard_pareto_frontier, augment_rare_classes, extract_column, compute_weighted_metric
 from autogluon.core.utils import get_pred_from_proba, get_pred_from_proba_df, infer_problem_type
 from autogluon.features.generators import PipelineFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
@@ -128,34 +130,52 @@
         self._validate_fit_input(X=X, X_val=X_val, **kwargs)
         return self._fit(X=X, X_val=X_val, **kwargs)
 
     def _fit(self, X: DataFrame, X_val: DataFrame = None, scheduler_options=None, hyperparameter_tune=False,
              feature_prune=False, holdout_frac=0.1, hyperparameters=None, verbosity=2):
         raise NotImplementedError
 
-    def predict_proba(self, X: DataFrame, model=None, as_pandas=True, as_multiclass=True, inverse_transform=True, transform_features=True):
+    def predict_proba(self,
+                      X: DataFrame,
+                      model: str | None = None,
+                      as_pandas: bool = True,
+                      as_multiclass: bool = True,
+                      inverse_transform: bool = True,
+                      transform_features: bool = True):
         X_index = copy.deepcopy(X.index) if as_pandas else None
         if X.empty:
             y_pred_proba = np.array([])
         else:
             if transform_features:
                 X = self.transform_features(X)
             y_pred_proba = self.load_trainer().predict_proba(X, model=model)
         y_pred_proba = self._post_process_predict_proba(y_pred_proba=y_pred_proba,
                                                         as_pandas=as_pandas,
                                                         index=X_index,
                                                         as_multiclass=as_multiclass,
                                                         inverse_transform=inverse_transform)
         return y_pred_proba
 
-    def predict(self, X: DataFrame, model=None, as_pandas=True, inverse_transform=True, transform_features=True):
+    def predict(self,
+                X: DataFrame,
+                model: str | None = None,
+                as_pandas: bool = True,
+                inverse_transform: bool = True,
+                transform_features: bool = True,
+                *,
+                decision_threshold: float | None = None,
+                ):
+        if decision_threshold is None:
+            decision_threshold = 0.5
         X_index = copy.deepcopy(X.index) if as_pandas else None
         y_pred_proba = self.predict_proba(X=X, model=model, as_pandas=False, as_multiclass=False, inverse_transform=False, transform_features=transform_features)
         problem_type = self.label_cleaner.problem_type_transform or self.problem_type
-        y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=problem_type)
+        y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba,
+                                     problem_type=problem_type,
+                                     decision_threshold=decision_threshold)
         y_pred = self._post_process_predict(y_pred=y_pred,
                                             as_pandas=as_pandas,
                                             index=X_index,
                                             inverse_transform=inverse_transform)
         return y_pred
 
     def _post_process_predict(
@@ -288,36 +308,50 @@
         return predict_proba_dict
 
     def predict_multi(self,
                       X: DataFrame = None,
                       models: List[str] = None,
                       as_pandas: bool = True,
                       transform_features: bool = True,
-                      inverse_transform: bool = True) -> dict:
+                      inverse_transform: bool = True,
+                      *,
+                      decision_threshold: float = None) -> dict:
         """
         Identical to predict_proba_multi, except returns predictions instead of probabilities.
         """
         predict_proba_dict = self.predict_proba_multi(X=X,
                                                       models=models,
                                                       as_pandas=as_pandas,
                                                       transform_features=transform_features,
                                                       inverse_transform=inverse_transform)
         predict_dict = {}
-        if as_pandas:
-            for m in predict_proba_dict:
-                predict_dict[m] = get_pred_from_proba_df(predict_proba_dict[m], problem_type=self.problem_type)
-        else:
-            for m in predict_proba_dict:
-                y_pred = get_pred_from_proba(predict_proba_dict[m], problem_type=self.problem_type)
-                predict_dict[m] = self._post_process_predict(y_pred=y_pred,
-                                                             as_pandas=as_pandas,
-                                                             index=None,
-                                                             inverse_transform=inverse_transform)
+        for m in predict_proba_dict:
+            predict_dict[m] = self.get_pred_from_proba(y_pred_proba=predict_proba_dict[m],
+                                                       decision_threshold=decision_threshold,
+                                                       inverse_transform=inverse_transform)
         return predict_dict
 
+    def get_pred_from_proba(self,
+                            y_pred_proba: np.ndarray | pd.DataFrame,
+                            decision_threshold: float | None = None,
+                            inverse_transform: bool = True) -> np.array | pd.Series:
+        if isinstance(y_pred_proba, pd.DataFrame):
+            y_pred = get_pred_from_proba_df(y_pred_proba,
+                                            problem_type=self.problem_type,
+                                            decision_threshold=decision_threshold)
+        else:
+            y_pred = get_pred_from_proba(y_pred_proba,
+                                         problem_type=self.problem_type,
+                                         decision_threshold=decision_threshold)
+            y_pred = self._post_process_predict(y_pred=y_pred,
+                                                as_pandas=False,
+                                                index=None,
+                                                inverse_transform=inverse_transform)
+        return y_pred
+
     def _validate_fit_input(self, X: DataFrame, **kwargs):
         if self.label not in X.columns:
             raise KeyError(f"Label column '{self.label}' is missing from training data. Training data columns: {list(X.columns)}")
         X_val = kwargs.get('X_val', None)
         self._validate_sample_weight(X, X_val)
         self._validate_groups(X, X_val)
 
@@ -421,15 +455,16 @@
             y_pred = self.predict(X=X, model=model, as_pandas=False)
         else:
             y_pred = self.predict_proba(X=X, model=model, as_pandas=False, as_multiclass=False)
             y = self.label_cleaner.transform(y)
         return compute_weighted_metric(y, y_pred, self.eval_metric, w, weight_evaluation=self.weight_evaluation, quantile_levels=self.quantile_levels)
 
     # Scores both learner and all individual models, along with computing the optimal ensemble score + weights (oracle)
-    def score_debug(self, X: DataFrame, y=None, extra_info=False, compute_oracle=False, extra_metrics=None, skip_score=False, silent=False):
+    def score_debug(self, X: DataFrame, y=None, extra_info=False, compute_oracle=False, extra_metrics=None,
+                    decision_threshold=None, skip_score=False, silent=False):
         leaderboard_df = self.leaderboard(extra_info=extra_info, silent=silent)
         if extra_metrics is None:
             extra_metrics = []
         if y is None:
             error_if_missing = extra_metrics or not skip_score
             X, y = self.extract_label(X, error_if_missing=error_if_missing)
         w = None
@@ -475,23 +510,25 @@
         for model_name, y_pred_proba_internal in model_pred_proba_dict.items():
             if skip_score:
                 scores[model_name] = np.nan
             else:
                 scores[model_name] = self._score_with_pred_proba(
                     y_pred_proba_internal=y_pred_proba_internal,
                     metric=self.eval_metric,
+                    decision_threshold=decision_threshold,
                     **scoring_args
                 )
             for metric in extra_metrics:
                 metric = get_metric(metric, self.problem_type, 'leaderboard_metric')
                 if metric.name not in extra_scores:
                     extra_scores[metric.name] = {}
                 extra_scores[metric.name][model_name] = self._score_with_pred_proba(
                     y_pred_proba_internal=y_pred_proba_internal,
                     metric=metric,
+                    decision_threshold=decision_threshold,
                     **scoring_args
                 )
 
         if extra_scores:
             series = []
             for metric in extra_scores:
                 series.append(pd.Series(extra_scores[metric], name=metric))
@@ -568,22 +605,25 @@
 
     def _score_with_pred_proba(self,
                                y,
                                y_internal,
                                y_pred_proba_internal,
                                metric,
                                sample_weight=None,
+                               decision_threshold=None,
                                weight_evaluation=None):
         metric = get_metric(metric, self.problem_type, 'leaderboard_metric')
         if weight_evaluation is None:
             weight_evaluation = self.weight_evaluation
         if metric.needs_pred:
             if self.problem_type == BINARY:
                 # Use 1 and 0, otherwise f1 can crash due to unknown pos_label.
-                y_pred = get_pred_from_proba(y_pred_proba_internal, problem_type=self.problem_type)
+                y_pred = self.get_pred_from_proba(y_pred_proba_internal,
+                                                  decision_threshold=decision_threshold,
+                                                  inverse_transform=False)
                 y_tmp = y_internal
             else:
                 y_pred = self.label_cleaner.inverse_transform_proba(y_pred_proba_internal, as_pred=True)
                 y_tmp = y
         elif metric.needs_quantile:
             y_pred = self.label_cleaner.inverse_transform_proba(y_pred_proba_internal, as_pred=True)
             y_tmp = y
@@ -622,15 +662,15 @@
             for cls in y_unique:
                 if cls not in valid_class_set:
                     unknown_classes.append(cls)
             if unknown_classes:
                 # log_loss / pac_score
                 raise ValueError(f'Multiclass scoring with eval_metric=\'{self.eval_metric.name}\' does not support unknown classes. Unknown classes: {unknown_classes}')
 
-    def evaluate_predictions(self, y_true, y_pred, sample_weight=None, silent=False, auxiliary_metrics=True, detailed_report=False):
+    def evaluate_predictions(self, y_true, y_pred, sample_weight=None, decision_threshold=None, silent=False, auxiliary_metrics=True, detailed_report=False):
         """ Evaluate predictions. Does not support sample weights since this method reports a variety of metrics.
             Args:
                 silent (bool): Should we print which metric is being used as well as performance.
                 auxiliary_metrics (bool): Should we compute other (problem_type specific) metrics in addition to the default metric?
                 detailed_report (bool): Should we computed more-detailed versions of the auxiliary_metrics? (requires auxiliary_metrics=True).
 
             Returns single performance-value if auxiliary_metrics=False.
@@ -653,15 +693,15 @@
             raise AssertionError(f'`evaluate_predictions` requires y_pred_proba input '
                                  f'when evaluating "{self.eval_metric.name}"... Please generate valid input via `predictor.predict_proba(data)`.\n'
                                  f'This may have occurred if you passed in predict input instead of predict_proba input, '
                                  f'or if you specified `as_multiclass=False` to `predictor.predict_proba(data, as_multiclass=False)`, '
                                  f'which is not supported by `evaluate_predictions`.')
         if is_proba:
             y_pred_proba = y_pred
-            y_pred = get_pred_from_proba_df(y_pred_proba, problem_type=self.problem_type)
+            y_pred = self.get_pred_from_proba(y_pred_proba=y_pred_proba, decision_threshold=decision_threshold)
             if self.problem_type == BINARY:
                 # roc_auc crashes if this isn't done
                 y_pred_proba = y_pred_proba[self.positive_class]
         else:
             y_pred_proba = None
             y_pred = pd.Series(y_pred)
         if y_pred_proba is not None:
@@ -719,14 +759,15 @@
                 continue
 
             if aux_metric.name not in performance_dict:
                 if y_pred_proba_internal is not None:
                     score = self._score_with_pred_proba(
                         y_pred_proba_internal=y_pred_proba_internal,
                         metric=aux_metric,
+                        decision_threshold=decision_threshold,
                         **scoring_args
                     )
                 else:
                     score = self._score_with_pred(
                         y_pred_internal=y_pred_internal,
                         metric=aux_metric,
                         **scoring_args
@@ -767,17 +808,19 @@
                 raise ValueError(f"Provided DataFrame does not contain label column: {self.label}")
             else:
                 return X, None
         y = X[self.label].copy()
         X = X.drop(self.label, axis=1)
         return X, y
 
-    def leaderboard(self, X=None, y=None, extra_info=False, extra_metrics=None, only_pareto_frontier=False, skip_score=False, silent=False):
+    def leaderboard(self, X=None, y=None, extra_info=False, extra_metrics=None, decision_threshold=None,
+                    only_pareto_frontier=False, skip_score=False, silent=False) -> pd.DataFrame:
         if X is not None:
-            leaderboard = self.score_debug(X=X, y=y, extra_info=extra_info, extra_metrics=extra_metrics, skip_score=skip_score, silent=True)
+            leaderboard = self.score_debug(X=X, y=y, extra_info=extra_info, extra_metrics=extra_metrics,
+                                           decision_threshold=decision_threshold, skip_score=skip_score, silent=True)
         else:
             if extra_metrics:
                 raise AssertionError('`extra_metrics` is only valid when data is specified.')
             trainer = self.load_trainer()
             leaderboard = trainer.leaderboard(extra_info=extra_info)
         if only_pareto_frontier:
             if 'score_test' in leaderboard.columns and 'pred_time_test' in leaderboard.columns:
@@ -891,14 +934,55 @@
         trainer = self.load_trainer()
         distilled_model_names = trainer.distill(X=X, y=y, X_val=X_val, y_val=y_val, time_limit=time_limit, hyperparameters=hyperparameters,
                                                 holdout_frac=holdout_frac, verbosity=verbosity, teacher_preds=teacher_preds, models_name_suffix=models_name_suffix,
                                                 augmentation_data=augmentation_data, augment_method=augment_method, augment_args=augment_args)
         self.save_trainer(trainer=trainer)
         return distilled_model_names
 
+    def transform_labels(self, y, inverse=False, proba=False):
+        if inverse:
+            if proba:
+                y_transformed = self.label_cleaner.inverse_transform_proba(y=y, as_pandas=True)
+            else:
+                y_transformed = self.label_cleaner.inverse_transform(y=y)
+        else:
+            if proba:
+                y_transformed = self.label_cleaner.transform_proba(y=y, as_pandas=True)
+            else:
+                y_transformed = self.label_cleaner.transform(y=y)
+        return y_transformed
+
+    def calibrate_decision_threshold(self,
+                                     data: pd.DataFrame | None = None,
+                                     metric: str | Scorer | None = None,
+                                     model: str = 'best',
+                                     decision_thresholds: int | List[float] = 50,
+                                     verbose: bool = True) -> float:
+        # TODO: docstring
+        if metric is None:
+            metric = self.eval_metric
+
+        weights = None
+        if data is None:
+            X = None
+            y = None
+        else:
+            if self.weight_evaluation:
+                data, weights = extract_column(data, self.sample_weight)
+            X = self.transform_features(X=data)
+            y = self.transform_labels(y=data[self.label])
+
+        return self.load_trainer().calibrate_decision_threshold(X=X,
+                                                                y=y,
+                                                                metric=metric,
+                                                                model=model,
+                                                                weights=weights,
+                                                                decision_thresholds=decision_thresholds,
+                                                                verbose=verbose)
+
     # TODO: Add data info gathering at beginning of .fit() that is used by all learners to add to get_info output
     # TODO: Add feature inference / feature engineering info to get_info output
     def get_info(self, **kwargs):
         learner_info = {
             'path': self.path,
             'label': self.label,
             'random_state': self.random_state,
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 from .text_prediction.text_prediction_v1_model import TextPredictorModel
 from .image_prediction.image_predictor import ImagePredictorModel
 from .imodels.imodels_models import RuleFitModel, BoostedRulesModel, GreedyTreeModel, HSTreeModel, \
     FigsModel, _IModelsModel
 from .vowpalwabbit.vowpalwabbit_model import VowpalWabbitModel
 from .automm.automm_model import MultiModalPredictorModel
 from .automm.ft_transformer import FTTransformerModel
+from .tabpfn.tabpfn_model import TabPFNModel
+
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import inspect
 import logging
 import math
 import os
 import pprint
 import shutil
@@ -18,14 +20,15 @@
 from autogluon.common.utils.file_utils import get_directory_size, get_directory_size_per_file
 from autogluon.common.utils.log_utils import add_log_to_file, set_logger_verbosity
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.utils import setup_outputdir, get_autogluon_metadata, compare_autogluon_metadata, check_saved_predictor_version
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, AUTO_WEIGHT, BALANCE_WEIGHT, PSEUDO_MODEL_SUFFIX, PROBLEM_TYPES_CLASSIFICATION
 from autogluon.core.data.label_cleaner import LabelCleanerMulticlassToBinary
 from autogluon.core.dataset import TabularDataset
+from autogluon.core.metrics import Scorer
 from autogluon.core.problem_type import problem_type_info
 from autogluon.core.pseudolabeling.pseudolabeling import filter_pseudo, filter_ensemble_pseudo
 from autogluon.core.scheduler.scheduler_factory import scheduler_factory
 from autogluon.core.trainer import AbstractTrainer
 from autogluon.core.utils import get_pred_from_proba_df
 from autogluon.core.utils import plot_performance_vs_trials, plot_summary_of_models, plot_tabular_models
 from autogluon.core.utils.decorators import apply_presets
@@ -218,14 +221,15 @@
         self.verbosity = verbosity
         set_logger_verbosity(self.verbosity)
         if sample_weight == AUTO_WEIGHT:  # TODO: update auto_weight strategy and make it the default
             sample_weight = None
             logger.log(15, f"{AUTO_WEIGHT} currently does not use any sample weights.")
         self.sample_weight = sample_weight
         self.weight_evaluation = weight_evaluation  # TODO: sample_weight and weight_evaluation can both be properties that link to self._learner.sample_weight, self._learner.weight_evaluation
+        self._decision_threshold = None  # TODO: Each model should have its own decision threshold instead of one global threshold
         if self.sample_weight in [AUTO_WEIGHT, BALANCE_WEIGHT] and self.weight_evaluation:
             logger.warning(
                 f"We do not recommend specifying weight_evaluation when sample_weight='{self.sample_weight}', instead specify appropriate eval_metric.")
         self._validate_init_kwargs(kwargs)
         path = setup_outputdir(path)
         self._setup_log_to_file(
             path=path,
@@ -272,14 +276,48 @@
         self._assert_is_fit()
         return self._learner.original_features
 
     @property
     def problem_type(self):
         return self._learner.problem_type
 
+    @property
+    def decision_threshold(self) -> float:
+        """
+        The decision threshold used to convert prediction probabilities to predictions.
+        Only relevant for binary classification, otherwise the value will be None.
+        Valid values are in the range [0.0, 1.0]
+        You can obtain an optimized `decision_threshold` by first calling `predictor.calibrate_decision_threshold()`.
+        Useful to set for metrics such as `balanced_accuracy` and `f1` as `0.5` is often not an optimal threshold.
+        Predictions are calculated via the following logic on the positive class: `1 if pred > decision_threshold else 0`
+        """
+        if self._decision_threshold is not None:
+            return self._decision_threshold
+        elif self.problem_type == BINARY:
+            return 0.5
+        else:
+            return None
+
+    def set_decision_threshold(self, decision_threshold: float):
+        """
+        Set `predictor.decision_threshold`. Problem type must be 'binary', and the value must be between 0 and 1.
+        """
+        assert self.problem_type == BINARY
+        assert decision_threshold >= 0
+        assert decision_threshold <= 1
+        if decision_threshold != self.decision_threshold:
+            logger.log(20, f'Updating predictor.decision_threshold from {self.decision_threshold} -> {decision_threshold}\n'
+                           f'\tThis will impact how prediction probabilities are converted to predictions in binary classification.\n'
+                           f'\tPrediction probabilities of the positive class >{decision_threshold} '
+                           f'will be predicted as the positive class ({self.positive_class}). '
+                           f'This can significantly impact metric scores.\n'
+                           f'\tYou can update this value via `predictor.set_decision_threshold`.\n'
+                           f'\tYou can calculate an optimal decision threshold on the validation data via `predictor.calibrate_decision_threshold()`.')
+        self._decision_threshold = decision_threshold
+
     def features(self, feature_stage: str = 'original'):
         """
         Returns a list of feature names dependent on the value of feature_stage.
 
         Parameters
         ----------
         feature_stage : str, default = 'original'
@@ -320,14 +358,15 @@
             time_limit=None,
             presets=None,
             hyperparameters=None,
             feature_metadata='infer',
             infer_limit=None,
             infer_limit_batch_size=None,
             fit_weighted_ensemble=True,
+            calibrate_decision_threshold=False,
             num_cpus='auto',
             num_gpus='auto',
             **kwargs):
         """
         Fit models to predict a column of a data table (label) based on the other columns (features).
 
         Parameters
@@ -566,14 +605,20 @@
             Small values, especially `infer_limit_batch_size=1`, will result in much larger per-row inference times and should be avoided if possible.
             Refer to `infer_limit` for more details on how this is used.
             If specified when `infer_limit=None`, the inference time will be logged during training but will not be limited.
         fit_weighted_ensemble : bool, default = True
             If True, a WeightedEnsembleModel will be fit in each stack layer.
             A weighted ensemble will often be stronger than an individual model while being very fast to train.
             It is recommended to keep this value set to True to maximize predictive quality.
+        calibrate_decision_threshold : bool, default = False
+            [Experimental] This may be removed / changed without warning in a future release.
+            If True, will automatically calibrate the decision threshold at the end of fit for calls to `.predict` based on the evaluation metric.
+            By default, the decision threshold is `0.5`, however for some metrics such as `f1` and `balanced_accuracy`,
+            scores can be significantly improved by choosing a threshold other than `0.5`.
+            Only valid for `problem_type='binary'`. Ignored for all other problem types.
         num_cpus: int, default = "auto"
             The total amount of cpus you want AutoGluon predictor to use.
             Auto means AutoGluon will make the decision based on the total number of cpus available and the model requirement for best performance.
             Users generally don't need to set this value
         num_gpus: int, default = "auto"
             The total amount of gpus you want AutoGluon predictor to use.
             Auto means AutoGluon will make the decision based on the total number of gpus available and the model requirement for best performance.
@@ -896,21 +941,22 @@
 
         self._post_fit(
             keep_only_best=kwargs['keep_only_best'],
             refit_full=kwargs['refit_full'],
             set_best_to_refit_full=kwargs['set_best_to_refit_full'],
             save_space=kwargs['save_space'],
             calibrate=kwargs['calibrate'],
+            calibrate_decision_threshold=calibrate_decision_threshold,
             infer_limit=infer_limit,
         )
         self.save()
         return self
 
     def _post_fit(self, keep_only_best=False, refit_full=False, set_best_to_refit_full=False, save_space=False,
-                  calibrate=False, infer_limit=None):
+                  calibrate=False, calibrate_decision_threshold=False, infer_limit=None):
         if refit_full is True:
             if keep_only_best is True:
                 if set_best_to_refit_full is True:
                     refit_full = 'best'
                 else:
                     logger.warning(
                         f'refit_full was set to {refit_full}, but keep_only_best=True and set_best_to_refit_full=False. Disabling refit_full to avoid training models which would be automatically deleted.')
@@ -950,14 +996,21 @@
             if self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
                 self._trainer.calibrate_model()
             elif self.problem_type == QUANTILE:
                 self._trainer.calibrate_model()
             else:
                 logger.log(30, 'WARNING: `calibrate=True` is only applicable to classification or quantile regression problems. Skipping calibration...')
 
+        if calibrate_decision_threshold:
+            if self.problem_type != BINARY:
+                logger.log(30, 'WARNING: `calibrate_decision_threshold=True` is only applicable to binary classification. Skipping calibration...')
+            else:
+                best_threshold = self.calibrate_decision_threshold()
+                self.set_decision_threshold(decision_threshold=best_threshold)
+
         if keep_only_best:
             self.delete_models(models_to_keep='best', dry_run=False)
 
         if save_space:
             self.save_space()
 
     # TODO: Consider adding infer_limit to fit_extra
@@ -1376,15 +1429,21 @@
             logger.log(20, 'Given test_data for pseudo labeling did not contain labels. '
                            'AutoGluon will assign pseudo labels to data and use it for extra training data...')
             return self._run_pseudolabeling(unlabeled_data=pseudo_data, max_iter=max_iter,
                                             return_pred_prob=return_pred_prob, use_ensemble=use_ensemble,
                                             fit_ensemble=fit_ensemble, fit_ensemble_every_iter=fit_ensemble_every_iter,
                                             **fit_extra_kwargs)
 
-    def predict(self, data, model=None, as_pandas=True, transform_features=True):
+    def predict(self,
+                data: str | TabularDataset | pd.DataFrame,
+                model: str | None = None,
+                as_pandas: bool = True,
+                transform_features: bool = True,
+                *,
+                decision_threshold: float | None = None):
         """
         Use trained models to produce predictions of `label` column values for new data.
 
         Parameters
         ----------
         data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
             The data to make predictions for. Should contain same column names as training Dataset and follow same format
@@ -1395,24 +1454,39 @@
             Valid models are listed in this `predictor` by calling `predictor.get_model_names()`
         as_pandas : bool, default = True
             Whether to return the output as a :class:`pd.Series` (True) or :class:`np.ndarray` (False).
         transform_features : bool, default = True
             If True, preprocesses data before predicting with models.
             If False, skips global feature preprocessing.
                 This is useful to save on inference time if you have already called `data = predictor.transform_features(data)`.
+        decision_threshold : float, default = None
+            The decision threshold used to convert prediction probabilities to predictions.
+            Only relevant for binary classification, otherwise ignored.
+            If None, defaults to `predictor.decision_threshold`.
+            Valid values are in the range [0.0, 1.0]
+            You can obtain an optimized `decision_threshold` by first calling `predictor.calibrate_decision_threshold()`.
+            Useful to set for metrics such as `balanced_accuracy` and `f1` as `0.5` is often not an optimal threshold.
+            Predictions are calculated via the following logic on the positive class: `1 if pred > decision_threshold else 0`
 
         Returns
         -------
         Array of predictions, one corresponding to each row in given dataset. Either :class:`np.ndarray` or :class:`pd.Series` depending on `as_pandas` argument.
         """
         self._assert_is_fit('predict')
         data = self._get_dataset(data)
-        return self._learner.predict(X=data, model=model, as_pandas=as_pandas, transform_features=transform_features)
-
-    def predict_proba(self, data, model=None, as_pandas=True, as_multiclass=True, transform_features=True):
+        if decision_threshold is None:
+            decision_threshold = self.decision_threshold
+        return self._learner.predict(X=data, model=model, as_pandas=as_pandas, transform_features=transform_features, decision_threshold=decision_threshold)
+
+    def predict_proba(self,
+                      data: str | TabularDataset | pd.DataFrame,
+                      model: str | None = None,
+                      as_pandas: bool = True,
+                      as_multiclass: bool = True,
+                      transform_features: bool = True):
         """
         Use trained models to produce predicted class probabilities rather than class-labels (if task is classification).
         If `predictor.problem_type` is regression or quantile, this will raise an AssertionError.
 
         Parameters
         ----------
         data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
@@ -1447,37 +1521,82 @@
         if not self.can_predict_proba:
             raise AssertionError(f'`predictor.predict_proba` is not supported when problem_type="{self.problem_type}". '
                                  f'Please call `predictor.predict` instead. '
                                  f'You can check the value of `predictor.can_predict_proba` to tell if predict_proba is valid.')
         data = self._get_dataset(data)
         return self._learner.predict_proba(X=data, model=model, as_pandas=as_pandas, as_multiclass=as_multiclass, transform_features=transform_features)
 
+    def get_pred_from_proba(self,
+                            y_pred_proba: pd.DataFrame | np.ndarray,
+                            decision_threshold: float | None = None) -> pd.Series | np.array:
+        """
+        Given prediction probabilities, convert to predictions.
+
+        Parameters
+        ----------
+        y_pred_proba : :class:`pd.DataFrame` or :class:`np.ndarray`
+            The prediction probabilities to convert to predictions.
+            Obtainable via the output of `predictor.predict_proba`.
+        decision_threshold : float, default = None
+            The decision threshold used to convert prediction probabilities to predictions.
+            Only relevant for binary classification, otherwise ignored.
+            If None, defaults to `predictor.decision_threshold`.
+            Valid values are in the range [0.0, 1.0]
+            You can obtain an optimized `decision_threshold` by first calling `predictor.calibrate_decision_threshold()`.
+            Useful to set for metrics such as `balanced_accuracy` and `f1` as `0.5` is often not an optimal threshold.
+            Predictions are calculated via the following logic on the positive class: `1 if pred > decision_threshold else 0`
+
+        Returns
+        -------
+        Array of predictions, one corresponding to each row in given dataset. Either :class:`np.ndarray` or :class:`pd.Series` depending on `y_pred_proba` dtype.
+
+        Examples
+        --------
+        >>> from autogluon.tabular import TabularPredictor
+        >>> predictor = TabularPredictor(label='class').fit('train.csv', label='class')
+        >>> y_pred_proba = predictor.predict_proba('test.csv')
+        >>>
+        >>> # y_pred and y_pred_from_proba are identical
+        >>> y_pred = predictor.predict('test.csv')
+        >>> y_pred_from_proba = predictor.get_pred_from_proba(y_pred_proba=y_pred_proba)
+        """
+        if not self.can_predict_proba:
+            raise AssertionError(f'`predictor.get_pred_from_proba` is not supported when problem_type="{self.problem_type}".')
+        if decision_threshold is None:
+            decision_threshold = self.decision_threshold
+        return self._learner.get_pred_from_proba(y_pred_proba=y_pred_proba, decision_threshold=decision_threshold)
+
     @property
     def can_predict_proba(self) -> bool:
         """
         Return True if predictor can return prediction probabilities via `.predict_proba`, otherwise return False.
         Raises an AssertionError if called before fitting.
         """
         self._assert_is_fit('can_predict_proba')
         return problem_type_info.can_predict_proba(problem_type=self.problem_type)
 
-    def evaluate(self, data, model=None, silent=False, auxiliary_metrics=True, detailed_report=False) -> dict:
+    def evaluate(self, data, model=None, decision_threshold=None, silent=False, auxiliary_metrics=True, detailed_report=False) -> dict:
         """
         Report the predictive performance evaluated over a given dataset.
         This is basically a shortcut for: `pred_proba = predict_proba(data); evaluate_predictions(data[label], pred_proba)`.
 
         Parameters
         ----------
         data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
             This dataset must also contain the `label` with the same column-name as previously specified.
             If str is passed, `data` will be loaded using the str value as the file path.
             If `self.sample_weight` is set and `self.weight_evaluation==True`, then a column with the sample weight name is checked and used for weighted metric evaluation if it exists.
         model : str (optional)
             The name of the model to get prediction probabilities from. Defaults to None, which uses the highest scoring model on the validation set.
             Valid models are listed in this `predictor` by calling `predictor.get_model_names()`.
+        decision_threshold : float, default = None
+            The decision threshold to use when converting prediction probabilities to predictions.
+            This will impact the scores of metrics such as `f1` and `accuracy`.
+            If None, defaults to `predictor.decision_threshold`. Ignored unless `problem_type='binary'`.
+            Refer to the `predictor.decision_threshold` docstring for more information.
         silent : bool, default = False
             If False, performance results are printed.
         auxiliary_metrics: bool, default = True
             Should we compute other (`problem_type` specific) metrics in addition to the default metric?
         detailed_report : bool, default = False
             Should we computed more detailed versions of the `auxiliary_metrics`? (requires `auxiliary_metrics = True`)
 
@@ -1485,60 +1604,72 @@
         -------
         Returns dict where keys = metrics, values = performance along each metric. To get the `eval_metric` score, do `output[predictor.eval_metric.name]`
         NOTE: Metrics scores always show in higher is better form.
         This means that metrics such as log_loss and root_mean_squared_error will have their signs FLIPPED, and values will be negative.
         """
         self._assert_is_fit('evaluate')
         data = self._get_dataset(data)
+        if decision_threshold is None:
+            decision_threshold = self.decision_threshold
         if self.can_predict_proba:
             y_pred = self.predict_proba(data=data, model=model)
         else:
             y_pred = self.predict(data=data, model=model)
         if self.sample_weight is not None and self.weight_evaluation and self.sample_weight in data:
             sample_weight = data[self.sample_weight]
         else:
             sample_weight = None
-        return self.evaluate_predictions(y_true=data[self.label], y_pred=y_pred, sample_weight=sample_weight, silent=silent,
+        return self.evaluate_predictions(y_true=data[self.label], y_pred=y_pred, sample_weight=sample_weight,
+                                         decision_threshold=decision_threshold, silent=silent,
                                          auxiliary_metrics=auxiliary_metrics, detailed_report=detailed_report)
 
-    def evaluate_predictions(self, y_true, y_pred, sample_weight=None, silent=False, auxiliary_metrics=True, detailed_report=False) -> dict:
+    def evaluate_predictions(self, y_true, y_pred, sample_weight=None, decision_threshold=None, silent=False, auxiliary_metrics=True, detailed_report=False) -> dict:
         """
         Evaluate the provided prediction probabilities against ground truth labels.
         Evaluation is based on the `eval_metric` previously specified in init, or default metrics if none was specified.
 
         Parameters
         ----------
         y_true : :class:`np.array` or :class:`pd.Series`
             The ordered collection of ground-truth labels.
         y_pred : :class:`pd.Series` or :class:`pd.DataFrame`
             The ordered collection of prediction probabilities or predictions.
             Obtainable via the output of `predictor.predict_proba`.
             Caution: For certain types of `eval_metric` (such as 'roc_auc'), `y_pred` must be predicted-probabilities rather than predicted labels.
         sample_weight : :class:`pd.Series`, default = None
             Sample weight for each row of data. If None, uniform sample weights are used.
+        decision_threshold : float, default = None
+            The decision threshold to use when converting prediction probabilities to predictions.
+            This will impact the scores of metrics such as `f1` and `accuracy`.
+            If None, defaults to `predictor.decision_threshold`. Ignored unless `problem_type='binary'`.
+            Refer to the `predictor.decision_threshold` docstring for more information.
         silent : bool, default = False
             If False, performance results are printed.
         auxiliary_metrics: bool, default = True
             Should we compute other (`problem_type` specific) metrics in addition to the default metric?
         detailed_report : bool, default = False
             Should we computed more detailed versions of the `auxiliary_metrics`? (requires `auxiliary_metrics = True`)
 
         Returns
         -------
         Returns dict where keys = metrics, values = performance along each metric.
         NOTE: Metrics scores always show in higher is better form.
         This means that metrics such as log_loss and root_mean_squared_error will have their signs FLIPPED, and values will be negative.
         """
-        return self._learner.evaluate_predictions(y_true=y_true, y_pred=y_pred, sample_weight=sample_weight, silent=silent,
+        if decision_threshold is None:
+            decision_threshold = self.decision_threshold
+        return self._learner.evaluate_predictions(y_true=y_true, y_pred=y_pred, sample_weight=sample_weight,
+                                                  decision_threshold=decision_threshold, silent=silent,
                                                   auxiliary_metrics=auxiliary_metrics, detailed_report=detailed_report)
 
     def leaderboard(self,
-                    data=None,
+                    data: str | TabularDataset | pd.DataFrame | None = None,
                     extra_info: bool = False,
-                    extra_metrics: list = None,
+                    extra_metrics: list | None = None,
+                    decision_threshold: float | None = None,
                     only_pareto_frontier: bool = False,
                     skip_score: bool = False,
                     silent: bool = False) -> pd.DataFrame:
         """
         Output summary of information about models produced during `fit()` as a :class:`pd.DataFrame`.
         Includes information on test and validation scores for all models, model training times, inference times, and stack levels.
         Output DataFrame columns include:
@@ -1641,14 +1772,22 @@
             For example, `extra_metrics=['accuracy', 'roc_auc', 'log_loss']` would be valid in binary classification.
             This example would return 3 additional columns in the output DataFrame, whose column names match the names of the metrics.
             Passing `extra_metrics=[predictor.eval_metric]` would return an extra column in the name of the eval metric that has identical values to `score_test`.
             This also works with custom metrics. If passing an object instead of a string, the column name will be equal to the `.name` attribute of the object.
             NOTE: Metrics scores always show in higher is better form.
             This means that metrics such as log_loss and root_mean_squared_error will have their signs FLIPPED, and values will be negative.
             This is necessary to avoid the user needing to know the metric to understand if higher is better when looking at leaderboard.
+        decision_threshold : float, default = None
+            The decision threshold to use when converting prediction probabilities to predictions.
+            This will impact the scores of metrics such as `f1` and `accuracy`.
+            If None, defaults to `predictor.decision_threshold`. Ignored unless `problem_type='binary'`.
+            Refer to the `predictor.decision_threshold` docstring for more information.
+            NOTE: `score_val` will not be impacted by this value in v0.8.
+                `score_val` will always show the validation scores achieved with a decision threshold of `0.5`.
+                Only test scores will be properly updated.
         only_pareto_frontier : bool, default = False
             If `True`, only return model information of models in the Pareto frontier of the accuracy/latency trade-off (models which achieve the highest score within their end-to-end inference time).
             At minimum this will include the model with the highest score and the model with the lowest inference time.
             This is useful when deciding which model to use during inference if inference time is a consideration.
             Models filtered out by this process would never be optimal choices for a user that only cares about model inference time and score.
         skip_score : bool, default = False
             [Advanced, primarily for developers]
@@ -1659,15 +1798,17 @@
 
         Returns
         -------
         :class:`pd.DataFrame` of model performance summary information.
         """
         self._assert_is_fit('leaderboard')
         data = self._get_dataset(data, allow_nan=True)
-        return self._learner.leaderboard(X=data, extra_info=extra_info, extra_metrics=extra_metrics,
+        if decision_threshold is None:
+            decision_threshold = self.decision_threshold
+        return self._learner.leaderboard(X=data, extra_info=extra_info, extra_metrics=extra_metrics, decision_threshold=decision_threshold,
                                          only_pareto_frontier=only_pareto_frontier, skip_score=skip_score, silent=silent)
 
     def predict_proba_multi(self,
                             data=None,
                             models: List[str] = None,
                             as_pandas: bool = True,
                             as_multiclass: bool = True,
@@ -1733,15 +1874,17 @@
                                                  inverse_transform=inverse_transform)
 
     def predict_multi(self,
                       data=None,
                       models: List[str] = None,
                       as_pandas: bool = True,
                       transform_features: bool = True,
-                      inverse_transform: bool = True) -> dict:
+                      inverse_transform: bool = True,
+                      *,
+                      decision_threshold: float = None) -> dict:
         """
         Returns a dictionary of predictions where the key is
         the model name and the value is the model's prediction probabilities on the data.
 
         Equivalent output to:
         ```
         predict_dict = {}
@@ -1769,26 +1912,37 @@
         transform_features : bool, default = True
             If True, preprocesses data before predicting with models.
             If False, skips global feature preprocessing.
                 This is useful to save on inference time if you have already called `data = predictor.transform_features(data)`.
         inverse_transform : bool, default = True
             If True, will return predictions in the original format.
             If False (advanced), will return predictions in AutoGluon's internal format.
+        decision_threshold : float, default = None
+            The decision threshold used to convert prediction probabilities to predictions.
+            Only relevant for binary classification, otherwise ignored.
+            If None, defaults to `0.5`.
+            Valid values are in the range [0.0, 1.0]
+            You can obtain an optimized `decision_threshold` by first calling `predictor.calibrate_decision_threshold()`.
+            Useful to set for metrics such as `balanced_accuracy` and `f1` as `0.5` is often not an optimal threshold.
+            Predictions are calculated via the following logic on the positive class: `1 if pred > decision_threshold else 0`
 
         Returns
         -------
         Dictionary with model names as keys and model predictions as values.
         """
         self._assert_is_fit('predict_multi')
+        if decision_threshold is None:
+            decision_threshold = self.decision_threshold
         data = self._get_dataset(data, allow_nan=True)
         return self._learner.predict_multi(X=data,
                                            models=models,
                                            as_pandas=as_pandas,
                                            transform_features=transform_features,
-                                           inverse_transform=inverse_transform)
+                                           inverse_transform=inverse_transform,
+                                           decision_threshold=decision_threshold)
 
     def fit_summary(self, verbosity=3, show_plot=False):
         """
         Output summary of information about models produced during `fit()`.
         May create various generated summary plots and store them in folder: `predictor.path`.
 
         Parameters
@@ -2014,25 +2168,15 @@
 
         Returns
         -------
         :class:`pd.Series` of labels if `proba=False` or :class:`pd.DataFrame` of label probabilities if `proba=True`.
 
         """
         self._assert_is_fit('transform_labels')
-        if inverse:
-            if proba:
-                labels_transformed = self._learner.label_cleaner.inverse_transform_proba(y=labels, as_pandas=True)
-            else:
-                labels_transformed = self._learner.label_cleaner.inverse_transform(y=labels)
-        else:
-            if proba:
-                labels_transformed = self._learner.label_cleaner.transform_proba(y=labels, as_pandas=True)
-            else:
-                labels_transformed = self._learner.label_cleaner.transform(y=labels)
-        return labels_transformed
+        return self._learner.transform_labels(y=labels, inverse=inverse, proba=proba)
 
     def feature_importance(self, data=None, model=None, features=None, feature_stage='original', subsample_size=5000,
                            time_limit=None, num_shuffle_sets=None, include_confidence_band=True, confidence_level=0.99,
                            silent=False):
         """
         Calculates feature importance scores for the given model via permutation importance. Refer to https://explained.ai/rf-importance/ for an explanation of permutation importance.
         A feature's importance score represents the performance drop that results when the model makes predictions on a perturbed copy of the data where this feature's values have been randomly shuffled across rows.
@@ -2503,15 +2647,85 @@
                                                      name_suffix=name_suffix, time_limit=time_limit)
 
         if refit_full:
             models += self.refit_full(model=models)
 
         return models
 
-    def get_oof_pred(self, model: str = None, transformed=False, train_data=None, internal_oof=False, can_infer=None) -> pd.Series:
+    def calibrate_decision_threshold(self,
+                                     data: str | TabularDataset | pd.DataFrame | None = None,
+                                     metric: str | Scorer | None = None,
+                                     model: str = 'best',
+                                     decision_thresholds: int | List[float] = 50,
+                                     verbose: bool = True) -> float:
+        """
+        Calibrate the decision threshold in binary classification to optimize a given metric.
+        You can pass the output of this method as input to `predictor.set_decision_threshold` to update the predictor.
+        Will raise an AssertionError if `predictor.problem_type != 'binary'`.
+
+        Note that while calibrating the decision threshold can help to improve a given metric,
+        other metrics may end up having worse scores.
+        For example, calibrating on `balanced_accuracy` will often harm `accuracy`.
+        Users should keep this in mind while leveraging decision threshold calibration.
+
+        Parameters
+        ----------
+        data : Union[str, pd.DataFrame], default = None
+            The data to use for calibration. Must contain the label column.
+            We recommend to keep this value as None unless you are an advanced user and understand the implications.
+            If None, will use internal data such as the holdout validation data or out-of-fold predictions.
+        metric : autogluon.core.metrics.Scorer or str, default = None
+            The metric to optimize during calibration.
+            If None, uses `predictor.eval_metric`.
+        model : str, default = 'best'
+            The model to use prediction probabilities of when calibrating the threshold.
+            If 'best', will use `predictor.get_model_best()`.
+        decision_thresholds : Union[int, List[float]], default = 50
+            The number of decision thresholds on either side of `0.5` to search.
+            The default of 50 will result in 101 searched thresholds: [0.00, 0.01, 0.02, ..., 0.49, 0.50, 0.51, ..., 0.98, 0.99, 1.00]
+            Alternatively, a list of decision thresholds can be passed and only the thresholds in the list will be searched.
+        verbose : bool, default = True
+            If True, will log information about the calibration process.
+
+        Returns
+        -------
+        Decision Threshold: A float between 0 and 1 defining the decision boundary for predictions that
+        maximizes the `metric` score on the `data` for the `model`.
+        """
+        # TODO: v0.8
+        #  add tutorial section
+        #
+        # TODO: v0.9
+        #  Calculate optimal threshold for each model separately when deciding best model
+        #  sampling/time limit
+        #  update validation scores of models based on threshold
+        #  speed up the logic / search for optimal threshold more efficiently
+        #  make threshold calibration part of internal optimization, such as during fit_weighted_ensemble.
+        #  precision has strange edge-cases where it flips from 1.0 to 0.0 score due to becoming undefined
+        #    consider warning users who pass this metric,
+        #    or edit this metric so they do not flip value when undefined.
+        #      UndefinedMetricWarning: Precision is ill-defined and being set to 0.0 due to no predicted samples.
+        #      Use `zero_division` parameter to control this behavior.
+
+        self._assert_is_fit('calibrate_decision_threshold')
+        assert self.problem_type == BINARY, f'calibrate_decision_threshold is only available for `problem_type="{BINARY}"`'
+        data = self._get_dataset(data, allow_nan=True)
+
+        if metric is None:
+            metric = self.eval_metric
+        if model == 'best':
+            model = self.get_model_best()
+
+        return self._learner.calibrate_decision_threshold(data=data,
+                                                          metric=metric,
+                                                          model=model,
+                                                          decision_thresholds=decision_thresholds,
+                                                          verbose=verbose)
+
+    def get_oof_pred(self, model: str = None, transformed=False, train_data=None, internal_oof=False, decision_threshold=None, can_infer=None) -> pd.Series:
         """
         Note: This is advanced functionality not intended for normal usage.
 
         Returns the out-of-fold (OOF) predictions for every row in the training data.
 
         For more information, refer to `get_oof_pred_proba()` documentation.
 
@@ -2521,29 +2735,35 @@
             Refer to `get_oof_pred_proba()` documentation.
         transformed : bool, default = False
             Refer to `get_oof_pred_proba()` documentation.
         train_data : pd.DataFrame, default = None
             Refer to `get_oof_pred_proba()` documentation.
         internal_oof : bool, default = False
             Refer to `get_oof_pred_proba()` documentation.
+        decision_threshold : float, default = None
+            Refer to `predict_multi` documentation.
         can_infer : bool, default = None
             Refer to `get_oof_pred_proba()` documentation.
 
         Returns
         -------
         :class:`pd.Series` object of the out-of-fold training predictions of the model.
         """
         self._assert_is_fit('get_oof_pred')
+        if decision_threshold is None:
+            decision_threshold = self.decision_threshold
         y_pred_proba_oof = self.get_oof_pred_proba(model=model,
                                                    transformed=transformed,
                                                    as_multiclass=True,
                                                    train_data=train_data,
                                                    internal_oof=internal_oof,
                                                    can_infer=can_infer)
-        y_pred_oof = get_pred_from_proba_df(y_pred_proba_oof, problem_type=self.problem_type)
+        y_pred_oof = get_pred_from_proba_df(y_pred_proba_oof,
+                                            problem_type=self.problem_type,
+                                            decision_threshold=decision_threshold)
         if transformed:
             return self._learner.label_cleaner.to_transformed_dtype(y_pred_oof)
         return y_pred_oof
 
     # TODO: Improve error messages when trying to get oof from refit_full and distilled models.
     # TODO: v0.1 add tutorial related to this method, as it is very powerful.
     # TODO: Remove train_data argument once we start caching the raw original data: Can just load that instead.
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 from autogluon.core.models import AbstractModel, GreedyWeightedEnsembleModel, StackerEnsembleModel, SimpleWeightedEnsembleModel, DummyModel
 from autogluon.core.trainer.utils import process_hyperparameters
 
 from .presets_custom import get_preset_custom
 from ...models import LGBModel, CatBoostModel, XGBoostModel, RFModel, XTModel, KNNModel, LinearModel,\
     TabularNeuralNetTorchModel, NNFastAiTabularModel, FastTextModel, TextPredictorModel, \
     ImagePredictorModel, VowpalWabbitModel, \
-    RuleFitModel, GreedyTreeModel, HSTreeModel, FigsModel, BoostedRulesModel, MultiModalPredictorModel, FTTransformerModel
+    RuleFitModel, GreedyTreeModel, HSTreeModel, FigsModel, BoostedRulesModel, MultiModalPredictorModel, \
+    FTTransformerModel, TabPFNModel
 from ...models.tab_transformer.tab_transformer_model import TabTransformerModel
 
 logger = logging.getLogger(__name__)
 
 # Higher values indicate higher priority, priority dictates the order models are trained for a given level.
 DEFAULT_MODEL_PRIORITY = dict(
+    TABPFN=110,  # highest priority due to its very fast training time
     KNN=100,
     GBM=90,
     RF=80,
     CAT=70,
     XT=60,
     FASTAI=50,
     XGB=40,
@@ -73,15 +75,18 @@
     NN_TORCH=TabularNeuralNetTorchModel,
     LR=LinearModel,
     FASTAI=NNFastAiTabularModel,
     TRANSF=TabTransformerModel,
     AG_TEXT_NN=TextPredictorModel,
     AG_IMAGE_NN=ImagePredictorModel,
     AG_AUTOMM=MultiModalPredictorModel,
+
     FT_TRANSFORMER=FTTransformerModel,
+    TABPFN=TabPFNModel,
+
     FASTTEXT=FastTextModel,
     ENS_WEIGHTED=GreedyWeightedEnsembleModel,
     SIMPLE_ENS_WEIGHTED=SimpleWeightedEnsembleModel,
 
     # interpretable models
     IM_RULEFIT=RuleFitModel,
     IM_GREEDYTREE=GreedyTreeModel,
@@ -90,29 +95,33 @@
     IM_BOOSTEDRULES=BoostedRulesModel,
     VW=VowpalWabbitModel,
 
     DUMMY=DummyModel,
 )
 
 
+# TODO: v1.0 Have this be defined in the model class
 DEFAULT_MODEL_NAMES = {
     RFModel: 'RandomForest',
     XTModel: 'ExtraTrees',
     KNNModel: 'KNeighbors',
     LGBModel: 'LightGBM',
     CatBoostModel: 'CatBoost',
     XGBoostModel: 'XGBoost',
     TabularNeuralNetTorchModel: 'NeuralNetTorch',
     LinearModel: 'LinearModel',
     NNFastAiTabularModel: 'NeuralNetFastAI',
     TabTransformerModel: 'Transformer',
     TextPredictorModel: 'TextPredictor',
     ImagePredictorModel: 'ImagePredictor',
     MultiModalPredictorModel: 'MultiModalPredictor',
+
     FTTransformerModel: 'FTTransformer',
+    TabPFNModel: 'TabPFN',
+
     FastTextModel: 'FastText',
     VowpalWabbitModel: 'VowpalWabbit',
     GreedyWeightedEnsembleModel: 'WeightedEnsemble',
     SimpleWeightedEnsembleModel: 'WeightedEnsemble',
 
     # Interpretable models
     RuleFitModel: 'RuleFit',
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230612
+Version: 0.7.1b20230613
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -178,14 +178,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: lightgbm
 Provides-Extra: catboost
 Provides-Extra: xgboost
 Provides-Extra: fastai
+Provides-Extra: tabpfn
 Provides-Extra: ray
 Provides-Extra: skex
 Provides-Extra: imodels
 Provides-Extra: vowpalwabbit
 Provides-Extra: skl2onnx
 Provides-Extra: all
 Provides-Extra: tests
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,16 @@
 src/autogluon/tabular/models/tab_transformer/tab_transformer.py
 src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
 src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
 src/autogluon/tabular/models/tab_transformer/utils.py
 src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
 src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
 src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+src/autogluon/tabular/models/tabpfn/__init__.py
+src/autogluon/tabular/models/tabpfn/tabpfn_model.py
 src/autogluon/tabular/models/tabular_nn/__init__.py
 src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
 src/autogluon/tabular/models/tabular_nn/compilers/native.py
 src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
 src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
 src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
 src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
```

### Comparing `autogluon.tabular-0.7.1b20230612/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 numpy<1.27,>=1.21
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 networkx<3.0,>=2.3
-autogluon.core==0.7.1b20230612
-autogluon.features==0.7.1b20230612
+autogluon.core==0.7.1b20230613
+autogluon.features==0.7.1b20230613
 
 [all]
-torch<1.14,>=1.9
-fastai<2.8,>=2.3.1
-autogluon.core[all]==0.7.1b20230612
 catboost<1.3,>=1.1
-xgboost<1.8,>=1.6
+fastai<2.8,>=2.3.1
 lightgbm<3.4,>=3.3
+autogluon.core[all]==0.7.1b20230613
+torch<1.14,>=1.9
+xgboost<1.8,>=1.6
 
 [all:sys_platform == "darwin"]
 catboost<1.2,>=1.1
 
 [catboost]
 catboost<1.3,>=1.1
 
@@ -30,24 +30,28 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<3.4,>=3.3
 
 [ray]
-autogluon.core[all]==0.7.1b20230612
+autogluon.core[all]==0.7.1b20230613
 
 [skex]
 scikit-learn-intelex<2023.2,>=2021.7
 
 [skl2onnx]
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
 
+[tabpfn]
+tabpfn<0.2,>=0.1
+
 [tests]
+tabpfn<0.2,>=0.1
 imodels<1.4.0,>=1.3.10
 vowpalwabbit<9.5,>=9
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
 
 [vowpalwabbit]
 vowpalwabbit<9.5,>=9
```

