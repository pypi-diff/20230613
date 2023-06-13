# Comparing `tmp/autogluon.core-0.7.1b20230612.tar.gz` & `tmp/autogluon.core-0.7.1b20230613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.1b20230612.tar", last modified: Mon Jun 12 09:03:56 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.1b20230613.tar", last modified: Tue Jun 13 09:04:02 2023, max compression
```

## Comparing `autogluon.core-0.7.1b20230612.tar` & `autogluon.core-0.7.1b20230613.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.958708 autogluon.core-0.7.1b20230612/
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-12 09:03:56.958708 autogluon.core-0.7.1b20230612/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:03:56.958708 autogluon.core-0.7.1b20230612/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.942707 autogluon.core-0.7.1b20230612/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.942707 autogluon.core-0.7.1b20230612/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.946708 autogluon.core-0.7.1b20230612/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.946708 autogluon.core-0.7.1b20230612/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.946708 autogluon.core-0.7.1b20230612/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.946708 autogluon.core-0.7.1b20230612/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94180 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59825 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.950708 autogluon.core-0.7.1b20230612/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   170013 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.954708 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49597 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-12 09:03:34.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:03:56.946708 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:03:56.000000 autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.073779 autogluon.core-0.7.1b20230613/
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-13 09:04:02.073779 autogluon.core-0.7.1b20230613/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:04:02.073779 autogluon.core-0.7.1b20230613/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.061779 autogluon.core-0.7.1b20230613/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.061779 autogluon.core-0.7.1b20230613/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94180 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59825 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.069779 autogluon.core-0.7.1b20230613/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174249 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.073779 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.073779 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.073779 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50798 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-13 09:03:45.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 09:04:01.000000 autogluon.core-0.7.1b20230613/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:02.065779 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-13 09:04:02.000000 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 09:04:02.000000 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:02.000000 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:02.000000 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 09:04:02.000000 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:02.000000 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:02.000000 autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.1b20230612/PKG-INFO` & `autogluon.core-0.7.1b20230613/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230612
+Version: 0.7.1b20230613
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230612/setup.py` & `autogluon.core-0.7.1b20230613/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/__init__.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/constants.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/dataset.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/problem_type.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/space.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import logging
 import os
 import time
 from collections import defaultdict
 from typing import Dict, List, Union, Tuple, Optional
 
@@ -16,18 +18,20 @@
 from autogluon.common.utils.log_utils import convert_time_in_s_to_log_friendly
 from autogluon.common.utils.path_converter import PathConverter
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_torch
 
 from .utils import process_hyperparameters
 from ..augmentation.distill_utils import format_distillation_labels, augment_data
+from ..calibrate import calibrate_decision_threshold
 from ..calibrate.conformity_score import compute_conformity_score
 from ..calibrate.temperature_scaling import tune_temperature_scaling
 from ..constants import AG_ARGS, BINARY, MULTICLASS, REGRESSION, QUANTILE, SOFTCLASS, REFIT_FULL_NAME, REFIT_FULL_SUFFIX
 from ..data.label_cleaner import LabelCleanerMulticlassToBinary
+from ..metrics import get_metric, Scorer
 from ..models import AbstractModel, BaggedEnsembleModel, StackerEnsembleModel, WeightedEnsembleModel, GreedyWeightedEnsembleModel, SimpleWeightedEnsembleModel
 from ..utils import default_holdout_frac, get_pred_from_proba, generate_train_test_split, infer_eval_metric, compute_permutation_feature_importance, \
     extract_column, compute_weighted_metric, convert_pred_probas_to_df
 from ..utils.exceptions import TimeLimitExceeded, NotEnoughMemoryError, NoValidFeatures, NoGPUError, NotEnoughCudaMemoryError
 from ..utils.loaders import load_pkl
 from ..utils.savers import save_json, save_pkl
 from ..utils.feature_selection import FeatureSelector
@@ -642,14 +646,20 @@
         if self.eval_metric.needs_pred or self.eval_metric.needs_quantile:
             y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=self.problem_type)
         else:
             y_pred = y_pred_proba
         return compute_weighted_metric(y, y_pred, self.eval_metric, weights, weight_evaluation=self.weight_evaluation,
                                        quantile_levels=self.quantile_levels)
 
+    def _score_with_y_pred(self, y, y_pred, weights=None, metric=None) -> float:
+        if metric is None:
+            metric = self.eval_metric
+        return compute_weighted_metric(y, y_pred, metric=metric, weights=weights, weight_evaluation=self.weight_evaluation,
+                                       quantile_levels=self.quantile_levels)
+
     # TODO: Slow if large ensemble with many models, could cache output result to speed up cascades during inference
     def _construct_model_pred_order(self, models: List[str]) -> List[str]:
         """
         Constructs a list of model names in order of inference calls required to infer on all the models.
 
         Parameters
         ----------
@@ -1181,14 +1191,18 @@
                 for stack_column_prefix in model_loaded.stack_column_prefix_lst:
                     base_model_name = model_loaded.stack_column_prefix_to_model_map[stack_column_prefix]
                     self.model_graph.add_edge(base_model_name, model_loaded.name)
 
         self.save()
         return self.get_model_full_dict()
 
+    def get_refit_full_parent(self, model: str) -> str:
+        """Get refit full model's parent. If model does not have a parent, return `model`."""
+        return self.get_model_attribute(model=model, attribute='refit_full_parent', default=model)
+
     # TODO: Take best performance model with lowest inference
     def get_model_best(self, can_infer=None, allow_full=True, infer_limit=None):
         models = self.get_model_names(can_infer=can_infer)
         if not models:
             raise AssertionError('Trainer has no fit models that can infer.')
         models_full = self.get_models_attribute_dict(models=models, attribute='refit_full_parent')
         if not allow_full:
@@ -2378,14 +2392,17 @@
         If inverse=True, return dict of refit model -> parent model
         """
         model_full_dict = self.get_models_attribute_dict(attribute='refit_full_parent')
         if not inverse:
             model_full_dict = {parent: refit for refit, parent in model_full_dict.items()}
         return model_full_dict
 
+    def model_exists(self, model: str) -> bool:
+        return model in self.get_model_names()
+
     def _get_banned_model_names(self) -> list:
         """Gets all model names which would cause model files to be overwritten if a new model was trained with the name"""
         return self.get_model_names() + list(self._extra_banned_names)
 
     def leaderboard(self, extra_info=False):
         model_names = self.get_model_names()
         score_val = []
@@ -3042,7 +3059,68 @@
             if temp_scalar is None:
                 logger.log(15, f'Warning: Infinity found during calibration, skipping calibration on {model.name}! '
                                f'This can occur when the model is absolutely certain of a validation prediction (1.0 pred_proba).')
             else:
                 logger.log(15, f'Temperature term found is: {temp_scalar}')
                 model.params_aux["temperature_scalar"] = temp_scalar
                 model.save()
+
+    def calibrate_decision_threshold(self,
+                                     X: pd.DataFrame | None = None,
+                                     y: np.array | None = None,
+                                     metric: str | Scorer | None = None,
+                                     model: str = 'best',
+                                     weights=None,
+                                     decision_thresholds: int | List[float] = 50,
+                                     verbose: bool = True) -> float:
+        # TODO: Docstring
+        assert self.problem_type == BINARY, f'calibrate_decision_threshold is only available for `problem_type="{BINARY}"`'
+
+        if metric is None:
+            metric = self.eval_metric
+        elif isinstance(metric, str):
+            metric = get_metric(metric, self.problem_type, 'eval_metric')
+
+        if model == 'best':
+            model = self.get_model_best()
+
+        if y is None:
+            # If model is refit_full, use its parent to avoid over-fitting
+            model_parent = self.get_refit_full_parent(model=model)
+            if not self.model_exists(model_parent):
+                raise AssertionError(f'Unable to calibrate the decision threshold on the internal data because the '
+                                     f'model "{model}" is a refit_full model trained on all of the internal data, '
+                                     f'whose parent model "{model_parent}" does not exist or was deleted.\n'
+                                     f'It may have been deleted due to `predictor.fit(..., keep_only_best=True)`. '
+                                     f'Ensure `keep_only_best=False` to be able to calibrate refit_full models.')
+            model = model_parent
+
+            # TODO: Add helpful logging when data is not available, for example post optimize for deployment
+            if self.has_val:
+                # Use validation data
+                X = self.load_X_val()
+                if self.weight_evaluation:
+                    X, weights = extract_column(X=X, col_name=self.sample_weight)
+                y: np.array = self.load_y_val()
+                y_pred_proba = self.predict_proba(X=X, model=model)
+            else:
+                # Use out-of-fold data
+                if self.weight_evaluation:
+                    X = self.load_X()
+                    X, weights = extract_column(X=X, col_name=self.sample_weight)
+                y: np.array = self.load_y()
+                y_pred_proba = self.get_model_oof(model=model)
+        else:
+            y_pred_proba = self.predict_proba(X=X, model=model)
+
+        if not metric.needs_pred:
+            logger.warning(f'WARNING: The provided metric "{metric.name}" does not use class predictions for scoring, '
+                           f'and thus is invalid for decision threshold calibration. '
+                           f'Falling back to `decision_threshold=0.5`.')
+            return 0.5
+
+        return calibrate_decision_threshold(y=y,
+                                            y_pred_proba=y_pred_proba,
+                                            metric=lambda y, y_pred : self._score_with_y_pred(y=y, y_pred=y_pred, weights=weights, metric=metric),
+                                            decision_thresholds=decision_thresholds,
+                                            metric_name=metric.name,
+                                            verbose=verbose)
```

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import math
 import pickle
 import time
 import random
 import sys
-from typing import Callable, List, Tuple
+from typing import Callable, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import scipy.stats
 from numpy.typing import ArrayLike
 from pandas import DataFrame, Series
 from sklearn.model_selection import RepeatedKFold, RepeatedStratifiedKFold, LeaveOneGroupOut
@@ -249,36 +249,50 @@
     class_counts_invalid = class_counts[class_counts < threshold]
     class_counts_invalid = class_counts_invalid[~class_counts_invalid.index.isin(set(missing_classes))]
     if len(class_counts_invalid) > 0:
         raise RuntimeError("augment_rare_classes failed to produce enough data from rare classes")
     return X
 
 
-def get_pred_from_proba_df(y_pred_proba, problem_type=BINARY):
-    """From input DataFrame of pred_proba, return Series of pred"""
+def get_pred_from_proba_df(y_pred_proba: pd.DataFrame,
+                           problem_type: str = BINARY,
+                           decision_threshold: float = None) -> pd.Series:
+    """
+    From input DataFrame of pred_proba, return Series of pred.
+    The input DataFrame's columns must be the names of the target classes.
+    """
     if problem_type == REGRESSION:
         y_pred = y_pred_proba
     elif problem_type == QUANTILE:
         y_pred = y_pred_proba
+    elif problem_type == BINARY and decision_threshold is not None:
+        negative_class, positive_class = y_pred_proba.columns
+        y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba.values,
+                                     problem_type=problem_type,
+                                     decision_threshold=decision_threshold)
+        y_pred = [positive_class if pred == 1 else negative_class for pred in y_pred]
+        y_pred = pd.Series(data=y_pred, index=y_pred_proba.index)
     else:
         y_pred = y_pred_proba.idxmax(axis=1)
     return y_pred
 
 
-def get_pred_from_proba(y_pred_proba: np.ndarray, problem_type=BINARY):
+def get_pred_from_proba(y_pred_proba: np.ndarray, problem_type=BINARY, decision_threshold: float = None):
     if problem_type == BINARY:
+        if decision_threshold is None:
+            decision_threshold = 0.5
         # Using > instead of >= to align with Pandas `.idxmax` logic which picks the left-most column during ties.
         # If this is not done, then predictions can be inconsistent when converting in binary classification from multiclass-form pred_proba and
         # binary-form pred_proba when the pred_proba is 0.5 for positive and negative classes.
         if len(y_pred_proba.shape) == 2:
             assert y_pred_proba.shape[1] == 2
             # Assume positive class is in 2nd position
-            y_pred = [1 if pred > 0.5 else 0 for pred in y_pred_proba[:, 1]]
+            y_pred = [1 if pred > decision_threshold else 0 for pred in y_pred_proba[:, 1]]
         else:
-            y_pred = [1 if pred > 0.5 else 0 for pred in y_pred_proba]
+            y_pred = [1 if pred > decision_threshold else 0 for pred in y_pred_proba]
     elif problem_type == REGRESSION:
         y_pred = y_pred_proba
     elif problem_type == QUANTILE:
         y_pred = y_pred_proba
     else:
         y_pred = []
         if not len(y_pred_proba) == 0:
@@ -390,15 +404,15 @@
     test_data[label] = y_test
     return train_data, test_data
 
 
 def generate_train_test_split(X: DataFrame,
                               y: Series,
                               problem_type: str,
-                              test_size: float = 0.1,
+                              test_size: Union[float, int] = 0.1,
                               random_state=0,
                               min_cls_count_train=1) -> Tuple[DataFrame, DataFrame, Series, Series]:
     """
     Generate a train test split from input X, y.
     If you have a combined X, y DataFrame, refer to `generate_train_test_split_combined` instead.
 
     Parameters
@@ -410,30 +424,36 @@
         Used for stratification and to ensure all classes in multiclass classification are preserved in train data.
     problem_type : str
         The problem_type the label is used for. Determines if stratification is used.
         Options: ["binary", "multiclass", "regression", "softclass", "quantile"]
     test_size : float, default = 0.1
         The proportion of data to use for the test set.
         The remaining (1 - test_size) of data will be used for the training set.
+    test_size : float or int, default = 0.1
+        If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in the test split.
+        If int, represents the absolute number of test samples.
     random_state : int, default = 0
         Random seed to use during the split.
     min_cls_count_train : int, default = 1
         The minimum number of instances of each class that must occur in the training set (for classification).
         If not satisfied by the original split, instances of unsatisfied classes are
         taken from test and put into train until satisfied.
         Raises an exception if impossible to satisfy.
 
     Returns
     -------
     X_train, X_test, y_train, y_test : (DataFrame, DataFrame, Series, Series)
         The train_data and test_data after performing the split, separated into X and y.
 
     """
-    if (test_size <= 0.0) or (test_size >= 1.0):
-        raise ValueError("fraction of data to hold-out must be specified between 0 and 1")
+    if isinstance(test_size, float):
+        if (test_size <= 0.0) or (test_size >= 1.0):
+            raise ValueError("fraction of data to hold-out must be specified between 0 and 1")
+    elif isinstance(test_size, int):
+        assert test_size > 0
     valid_problem_types = [BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE]
     assert problem_type in valid_problem_types, f'Unknown problem type "{problem_type}" | Valid problem types: {valid_problem_types}'
 
     X_split = X
     y_split = y
     if problem_type in [BINARY, MULTICLASS]:
         stratify = y
```

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.1b20230613/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230612
+Version: 0.7.1b20230613
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230612/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.1b20230613/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/autogluon/core/dataset.py
 src/autogluon/core/problem_type.py
 src/autogluon/core/space.py
 src/autogluon/core/version.py
 src/autogluon/core/augmentation/__init__.py
 src/autogluon/core/augmentation/distill_utils.py
 src/autogluon/core/calibrate/__init__.py
+src/autogluon/core/calibrate/_decision_threshold.py
 src/autogluon/core/calibrate/conformity_score.py
 src/autogluon/core/calibrate/temperature_scaling.py
 src/autogluon/core/data/__init__.py
 src/autogluon/core/data/cleaner.py
 src/autogluon/core/data/label_cleaner.py
 src/autogluon/core/hpo/__init__.py
 src/autogluon/core/hpo/constants.py
```

