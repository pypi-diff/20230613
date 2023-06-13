# Comparing `tmp/ml-starter-0.0.55.tar.gz` & `tmp/ml-starter-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.55.tar", last modified: Sun Jun 11 18:59:41 2023, max compression
+gzip compressed data, was "ml-starter-0.0.56.tar", last modified: Tue Jun 13 21:27:21 2023, max compression
```

## Comparing `ml-starter-0.0.55.tar` & `ml-starter-0.0.56.tar`

### file list

```diff
@@ -1,162 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.949330 ml-starter-0.0.55/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 18:59:30.000000 ml-starter-0.0.55/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 18:59:30.000000 ml-starter-0.0.55/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-11 18:59:41.949330 ml-starter-0.0.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-11 18:59:30.000000 ml-starter-0.0.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.929329 ml-starter-0.0.55/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.933329 ml-starter-0.0.55/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.933329 ml-starter-0.0.55/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.933329 ml-starter-0.0.55/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.933329 ml-starter-0.0.55/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.933329 ml-starter-0.0.55/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.937330 ml-starter-0.0.55/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.937330 ml-starter-0.0.55/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.937330 ml-starter-0.0.55/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.937330 ml-starter-0.0.55/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.941330 ml-starter-0.0.55/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.941330 ml-starter-0.0.55/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.941330 ml-starter-0.0.55/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.941330 ml-starter-0.0.55/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.941330 ml-starter-0.0.55/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.941330 ml-starter-0.0.55/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.941330 ml-starter-0.0.55/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.945330 ml-starter-0.0.55/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.949330 ml-starter-0.0.55/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-06-11 18:59:30.000000 ml-starter-0.0.55/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:59:41.949330 ml-starter-0.0.55/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-11 18:59:41.000000 ml-starter-0.0.55/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-11 18:59:41.000000 ml-starter-0.0.55/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:59:41.000000 ml-starter-0.0.55/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-11 18:59:41.000000 ml-starter-0.0.55/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-11 18:59:41.000000 ml-starter-0.0.55/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-11 18:59:30.000000 ml-starter-0.0.55/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 18:59:30.000000 ml-starter-0.0.55/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-11 18:59:30.000000 ml-starter-0.0.55/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-11 18:59:30.000000 ml-starter-0.0.55/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-11 18:59:41.949330 ml-starter-0.0.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-11 18:59:30.000000 ml-starter-0.0.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 21:27:03.000000 ml-starter-0.0.56/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 21:27:03.000000 ml-starter-0.0.56/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 21:27:21.133587 ml-starter-0.0.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-13 21:27:03.000000 ml-starter-0.0.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.105587 ml-starter-0.0.56/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.105587 ml-starter-0.0.56/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.113587 ml-starter-0.0.56/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.117587 ml-starter-0.0.56/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.117587 ml-starter-0.0.56/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.117587 ml-starter-0.0.56/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.125587 ml-starter-0.0.56/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 21:27:03.000000 ml-starter-0.0.56/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 21:27:03.000000 ml-starter-0.0.56/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 21:27:03.000000 ml-starter-0.0.56/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 21:27:03.000000 ml-starter-0.0.56/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-13 21:27:21.137587 ml-starter-0.0.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-13 21:27:03.000000 ml-starter-0.0.56/setup.py
```

### Comparing `ml-starter-0.0.55/LICENSE` & `ml-starter-0.0.56/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/PKG-INFO` & `ml-starter-0.0.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.55
+Version: 0.0.56
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.55/README.md` & `ml-starter-0.0.56/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/api.py` & `ml-starter-0.0.56/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/core/common_types.py` & `ml-starter-0.0.56/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/core/config.py` & `ml-starter-0.0.56/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/core/env.py` & `ml-starter-0.0.56/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/core/registry.py` & `ml-starter-0.0.56/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/core/state.py` & `ml-starter-0.0.56/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/launchers/base.py` & `ml-starter-0.0.56/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/launchers/mp.py` & `ml-starter-0.0.56/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/launchers/slurm.py` & `ml-starter-0.0.56/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/launchers/torchrun.py` & `ml-starter-0.0.56/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/loggers/base.py` & `ml-starter-0.0.56/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/loggers/meter.py` & `ml-starter-0.0.56/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/loggers/multi.py` & `ml-starter-0.0.56/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/loggers/stdout.py` & `ml-starter-0.0.56/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/loggers/tensorboard.py` & `ml-starter-0.0.56/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/lr_schedulers/base.py` & `ml-starter-0.0.56/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/lr_schedulers/constant.py` & `ml-starter-0.0.56/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.56/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.56/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/lr_schedulers/linear.py` & `ml-starter-0.0.56/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.56/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.56/ml/lr_schedulers/scripts/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 
     python -m ml.lr_schedulers.scripts.plot linear /path/to/save.png
 """
 
 import argparse
 from pathlib import Path
 
-import matplotlib.pyplot as plt
-
 from ml.core.registry import register_lr_scheduler
 from ml.core.state import State
 from ml.utils.argparse import add_args, from_args
 
 
 def main() -> None:
     """Plots a learning rate schedule."""
+    try:
+        import matplotlib.pyplot as plt
+    except ImportError as e:
+        raise ImportError("Please install matplotlib to use this script: `pip install matplotlib`") from e
+
     # Gets the plotting-specific arguments.
     parser = argparse.ArgumentParser(description="Plots a learning rate schedule")
     parser.add_argument("lr_scheduler", help="Which scheduler to plot")
     parser.add_argument("save_path", help="Where to save the plot")
     parser.add_argument("-n", "--num-iters", type=int, default=100_000, help="Number of iterations")
     parser.add_argument("-s", "--stride", type=int, default=100, help="Stride between iterations")
     args, cli_args = parser.parse_known_args()
```

### Comparing `ml-starter-0.0.55/ml/models/activations.py` & `ml-starter-0.0.56/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/models/base.py` & `ml-starter-0.0.56/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/models/embeddings.py` & `ml-starter-0.0.56/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/models/init.py` & `ml-starter-0.0.56/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/models/kmeans.py` & `ml-starter-0.0.56/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/models/lora.py` & `ml-starter-0.0.56/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/models/norms.py` & `ml-starter-0.0.56/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/models/parallel.py` & `ml-starter-0.0.56/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/optimizers/adam.py` & `ml-starter-0.0.56/ml/optimizers/adam.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 
 
 @dataclass
 class AdamOptimizerConfig(BaseOptimizerConfig):
     lr: float = conf_field(1e-3, help="Learning rate")
     betas: tuple[float, float] = conf_field((0.9, 0.999), help="Beta coefficients")
-    eps: float = conf_field(1e-4, help="Epsilon term to add to the denominator for stability")
+    eps: float = conf_field(1e-8, help="Epsilon term to add to the denominator for stability")
     weight_decay: float = conf_field(0.0, help="Weight decay regularization to use")
     amsgrad: bool = conf_field(False, help="Whether to use the AMSGrad variant of the algorithm")
     foreach: bool = conf_field(False, help="Whether to use the foreach variant of the optimizer")
     capturable: bool = conf_field(False, help="Whether to use capturable AdamW pathway")
     differentiable: bool = conf_field(False, help="Whether to use differentiable AdamW")
     fused: bool = conf_field(False, help="Whether to use the fused optimizer")
```

### Comparing `ml-starter-0.0.55/ml/optimizers/adamw.py` & `ml-starter-0.0.56/ml/optimizers/adamw.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ml.optimizers.common import separate_decayable_params
 
 
 @dataclass
 class AdamWOptimizerConfig(BaseOptimizerConfig):
     lr: float = conf_field(1e-3, help="Learning rate")
     betas: tuple[float, float] = conf_field((0.9, 0.999), help="Beta coefficients")
-    eps: float = conf_field(1e-4, help="Epsilon term to add to the denominator for stability")
+    eps: float = conf_field(1e-8, help="Epsilon term to add to the denominator for stability")
     weight_decay: float = conf_field(1e-5, help="Weight decay regularization to use")
     amsgrad: bool = conf_field(False, help="Whether to use the AMSGrad variant of the algorithm")
     default_decay: bool = conf_field(True, help="Whether to decay module params which aren't explicitly specified")
     foreach: bool = conf_field(False, help="Whether to use the foreach variant of the optimizer")
     capturable: bool = conf_field(False, help="Whether to use capturable AdamW pathway")
     differentiable: bool = conf_field(False, help="Whether to use differentiable AdamW")
     fused: bool = conf_field(False, help="Whether to use the fused optimizer")
```

### Comparing `ml-starter-0.0.55/ml/optimizers/adan.py` & `ml-starter-0.0.56/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/optimizers/base.py` & `ml-starter-0.0.56/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/optimizers/common.py` & `ml-starter-0.0.56/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/optimizers/sgd.py` & `ml-starter-0.0.56/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/optimizers/shampoo.py` & `ml-starter-0.0.56/ml/optimizers/shampoo.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,40 +23,43 @@
     u, s, v = torch.svd(matrix)
     return (u @ s.pow_(power).diag() @ v.t()).to(device)
 
 
 class Shampoo(Optimizer):
     r"""Implements Shampoo Optimizer Algorithm.
 
-    This is taken from the `pytorch-optimizer` package.
+    This is taken from the ``pytorch-optimizer`` package.
 
-    It has been proposed in `Shampoo: Preconditioned Stochastic Tensor
-    Optimization`.
+    .. highlight:: python
+    .. code-block:: python
 
-    NOTE: This is *not* an implementation of the later paper, `Scalable Second
-    Order Optimization for Deep Learning`, which is becoming more popular.
+        import torch_optimizer as optim
+        optimizer = optim.Shampoo(model.parameters(), lr=0.01)
+        optimizer.zero_grad()
+        loss_fn(model(input), target).backward()
+        optimizer.step()
 
-    Arguments:
+    It has been proposed in ``Shampoo: Preconditioned Stochastic Tensor
+    Optimization``.
+
+    .. note::
+        This is *not* an implementation of the later paper, ``Scalable Second
+        Order Optimization for Deep Learning``, which is becoming more popular.
+
+    Parameters:
         params: iterable of parameters to optimize or dicts defining
             parameter groups
         lr: learning rate (default: 1e-3)
         momentum: momentum factor (default: 0)
         weight_decay: weight decay (L2 penalty) (default: 0)
         epsilon: epsilon added to each mat_gbar_j for numerical stability
             (default: 1e-4)
         update_freq: update frequency to compute inverse (default: 1)
 
-    Example:
-        >>> import torch_optimizer as optim
-        >>> optimizer = optim.Shampoo(model.parameters(), lr=0.01)
-        >>> optimizer.zero_grad()
-        >>> loss_fn(model(input), target).backward()
-        >>> optimizer.step()
-
-    Note:
+    .. note::
         Reference code: https://github.com/moskomule/shampoo.pytorch
     """
 
     def __init__(
         self,
         params: Params,
         lr: float = 1e-1,
@@ -105,14 +108,15 @@
                     continue
                 grad = p.grad.data
                 order = grad.ndimension()
                 original_size = grad.size()
                 state = self.state[p]
                 momentum = group["momentum"]
                 weight_decay = group["weight_decay"]
+
                 if len(state) == 0:
                     state["step"] = 0
                     if momentum > 0:
                         state["momentum_buffer"] = grad.clone()
                     for dim_id, dim in enumerate(grad.size()):
                         state[f"precond_{dim_id}"] = group["epsilon"] * torch.eye(dim, out=grad.new(dim, dim))
                         state[f"inv_precond_{dim_id}"] = grad.new(dim, dim).zero_()
```

### Comparing `ml-starter-0.0.55/ml/scripts/cli.py` & `ml-starter-0.0.56/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/scripts/stage.py` & `ml-starter-0.0.56/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/scripts/train.py` & `ml-starter-0.0.56/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/base.py` & `ml-starter-0.0.56/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.56/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.56/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/collate.py` & `ml-starter-0.0.56/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.56/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.56/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.56/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.56/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.56/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/utils.py` & `ml-starter-0.0.56/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.56/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/environments/base.py` & `ml-starter-0.0.56/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/environments/utils.py` & `ml-starter-0.0.56/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/environments/worker.py` & `ml-starter-0.0.56/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/losses/reduce.py` & `ml-starter-0.0.56/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/rl/base.py` & `ml-starter-0.0.56/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/rl/replay.py` & `ml-starter-0.0.56/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/tasks/sl/base.py` & `ml-starter-0.0.56/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/base.py` & `ml-starter-0.0.56/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/learning.py` & `ml-starter-0.0.56/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/compile.py` & `ml-starter-0.0.56/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.56/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.56/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.56/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.56/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.56/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.56/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.56/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.56/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.56/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/rl.py` & `ml-starter-0.0.56/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/trainers/sl.py` & `ml-starter-0.0.56/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/argparse.py` & `ml-starter-0.0.56/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/atomic.py` & `ml-starter-0.0.56/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/audio.py` & `ml-starter-0.0.56/ml/utils/audio.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 import shutil
 import warnings
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Iterator, Literal
 
 import av
-import ffmpeg
 import numpy as np
+import torch
+import torchaudio.functional as A
 from torch import Tensor
 
 from ml.utils.numpy import as_numpy_array
 
 
 @dataclass
 class AudioProps:
@@ -38,65 +39,82 @@
             sample_rate=stream.rate,
             channels=stream.channels,
             duration=stream.duration,
         )
 
     @classmethod
     def from_file_ffmpeg(cls, fpath: str | Path) -> "AudioProps":
+        try:
+            import ffmpeg
+        except ImportError as e:
+            raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+
         probe = ffmpeg.probe(str(fpath))
 
         for stream in probe["streams"]:
             if stream["codec_type"] == "audio":
                 return cls(
                     sample_rate=int(stream["sample_rate"]),
                     channels=int(stream["channels"]),
                     duration=float(stream["duration"]),
                 )
 
         raise ValueError(f"Could not find audio stream in {fpath}")
 
 
+def _cleanup_wav_chunk(wav: np.ndarray, channels: int | None = None) -> np.ndarray:
+    if wav.ndim == 1:
+        wav = wav.reshape(-1, 1 if channels is None else channels).T
+    return wav
+
+
 def read_audio_av(in_file: str | Path) -> Iterator[np.ndarray]:
     """Function that reads an audio file to a stream of numpy arrays using PyAV.
 
     Args:
         in_file: Path to the input file.
+
+    Yields:
+        Audio chunks as numpy arrays, with shape (n_channels, n_samples).
     """
+    props = AudioProps.from_file_av(in_file)
+
     container = av.open(str(in_file))
     stream = container.streams.audio[0]
 
     for frame in container.decode(stream):
-        yield frame.to_ndarray()
+        yield frame.to_ndarray().reshape(-1, props.channels).T
 
 
-def read_audio_ffmpeg(
-    in_file: str | Path,
-    *,
-    output_fmt: str = "f32le",
-    chunk_size: int = 16_000,
-) -> Iterator[np.ndarray]:
+def read_audio_ffmpeg(in_file: str | Path, *, chunk_size: int = 16_000) -> Iterator[np.ndarray]:
     """Function that reads an audio file to a stream of numpy arrays using FFMPEG.
 
     Args:
         in_file: Path to the input file.
-        output_fmt: Format of the output audio. See `ffmpeg` docs for more info.
         chunk_size: Size of the chunks to read.
 
     Yields:
-        Audio chunks as numpy arrays.
+        Audio chunks as numpy arrays, with shape (n_channels, n_samples).
     """
+    props = AudioProps.from_file_ffmpeg(in_file)
+
+    try:
+        import ffmpeg
+    except ImportError as e:
+        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+
     stream = ffmpeg.input(str(in_file))
-    stream = ffmpeg.output(stream, "pipe:", format=output_fmt, acodec="pcm_f32le")
-    stream = ffmpeg.run_async(stream, pipe_stdout=True)
+    stream = ffmpeg.output(stream, "pipe:", format="f32le", acodec="pcm_f32le")
+    stream = ffmpeg.run_async(stream, pipe_stdout=True, quiet=True)
 
     while True:
         chunk = stream.stdout.read(chunk_size)
         if not chunk:
             break
-        yield np.frombuffer(chunk, dtype=np.float32)
+        yield np.frombuffer(chunk, dtype=np.float32).reshape(props.channels, -1)
 
     stream.stdout.close()
     stream.wait()
 
 
 def write_audio_av(itr: Iterator[np.ndarray | Tensor], out_file: str | Path, sampling_rate: int) -> None:
     """Function that writes a stream of audio to a file using PyAV.
@@ -108,108 +126,163 @@
     """
     container = av.open(str(out_file), mode="w")
     stream = container.add_stream("pcm_f32le", rate=sampling_rate)
 
     is_first_frame = True
     is_mono = True
     for frame in itr:
-        frame_np_float = as_numpy_array(frame)
+        frame_np_float = _cleanup_wav_chunk(as_numpy_array(frame))
         assert frame_np_float.ndim == 2, f"Expected 2D array, got {frame_np_float.shape}D"
 
         if is_first_frame:
             assert (channels := frame_np_float.shape[0]) in (1, 2), f"Expected 1 or 2 channels, got {channels}"
             is_mono = channels == 1
             stream.channels = channels
             stream.layout = "mono" if is_mono else "stereo"
             is_first_frame = False
 
         frame_np = (frame_np_float * 2**15).astype(np.int16)
-        if is_mono:
-            frame_av = av.AudioFrame.from_ndarray(frame_np, format="s16")
-        else:
-            frame_av = av.AudioFrame.from_ndarray(frame_np, format="s16p")
+        output_fmt = "s16" if is_mono else "s16p"
+        frame_av = av.AudioFrame.from_ndarray(frame_np, format=output_fmt)
         frame_av.rate = sampling_rate
         frame_av.time_base = stream.time_base
         container.mux(stream.encode(frame_av))
 
     container.close()
 
 
 def write_audio_ffmpeg(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     sampling_rate: int,
-    *,
-    output_fmt: str = "f32le",
 ) -> None:
     """Function that writes a stream of audio to a file using FFMPEG.
 
     Args:
         itr: Iterator of audio chunks.
         out_file: Path to the output file.
         sampling_rate: Sampling rate of the audio.
-        output_fmt: Format of the output audio. See `ffmpeg` docs for more info.
     """
-    first_frame = as_numpy_array(next(itr))
-    assert first_frame.ndim == 2, f"Expected 2D array, got {first_frame.shape}D"
+    first_frame = _cleanup_wav_chunk(as_numpy_array(next(itr)))
     assert (channels := first_frame.shape[0]) in (1, 2), f"Expected 1 or 2 channels, got {channels}"
 
-    stream = ffmpeg.input("pipe:", format=output_fmt, acodec="pcm_f32le", ar=sampling_rate, ac=channels)
+    try:
+        import ffmpeg
+    except ImportError as e:
+        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+
+    stream = ffmpeg.input("pipe:", format="f32le", acodec="pcm_f32le", ar=sampling_rate, ac=channels)
     stream = ffmpeg.output(stream, str(out_file))
     stream = ffmpeg.overwrite_output(stream)
-    stream = ffmpeg.run_async(stream, pipe_stdin=True)
+    stream = ffmpeg.run_async(stream, pipe_stdin=True, quiet=True)
+
+    def get_bytes(frame: np.ndarray) -> bytes:
+        return frame.tobytes()
 
-    stream.stdin.write(first_frame.tobytes())
+    stream.stdin.write(get_bytes(first_frame))
     for frame in itr:
-        assert frame.ndim == 2, f"Expected 2D array, got {frame.shape}D"
-        assert frame.shape[0] == channels, f"Expected {channels} channels, got {frame.shape[0]}"
-        stream.stdin.write(as_numpy_array(frame).tobytes())
+        frame = _cleanup_wav_chunk(as_numpy_array(frame))
+        stream.stdin.write(get_bytes(frame))
 
     stream.stdin.close()
     stream.wait()
 
 
-Reader = Literal["ffmpeg", "av"]
-Writer = Literal["ffmpeg", "av"]
+Reader = Literal["ffmpeg", "av", "sf"]
+Writer = Literal["ffmpeg", "av", "sf"]
 
 
-def get_audio_props(in_file: str | Path, *, reader: Reader = "ffmpeg") -> AudioProps:
+def get_audio_props(in_file: str | Path, *, reader: Reader = "av") -> AudioProps:
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in this system.")
             reader = "av"
         else:
             return AudioProps.from_file_ffmpeg(in_file)
 
     if reader == "av":
         return AudioProps.from_file_av(in_file)
 
     raise ValueError(f"Unknown reader {reader}")
 
 
-def read_audio(in_file: str | Path, *, reader: Reader = "ffmpeg") -> Iterator[np.ndarray]:
+def _resample_audio(
+    audio_chunks: Iterator[np.ndarray],
+    *,
+    chunk_length: int | None = None,
+    sampling_rate: tuple[int, int] | None = None,
+) -> Iterator[np.ndarray]:
+    if chunk_length is None:
+        yield from audio_chunks
+        return
+
+    audio_chunk_list: list[np.ndarray] = []
+    total_length: int = 0
+    for chunk in audio_chunks:
+        if sampling_rate is not None:
+            chunk = A.resample(torch.from_numpy(chunk), sampling_rate[0], sampling_rate[1]).numpy()
+        cur_chunk_length = chunk.shape[-1]
+        while total_length + cur_chunk_length >= chunk_length:
+            yield np.concatenate(audio_chunk_list + [chunk[..., : chunk_length - total_length]], axis=-1)
+            chunk = chunk[..., chunk_length - total_length :]
+            audio_chunk_list = []
+            total_length = 0
+            cur_chunk_length = chunk.shape[-1]
+        if cur_chunk_length > 0:
+            audio_chunk_list.append(chunk)
+            total_length += cur_chunk_length
+
+    if audio_chunk_list:
+        yield np.concatenate(audio_chunk_list, axis=-1)
+
+
+def read_audio(
+    in_file: str | Path,
+    *,
+    chunk_length: int | None = None,
+    sampling_rate: int | None = None,
+    reader: Reader = "av",
+) -> Iterator[np.ndarray]:
+    """Function that reads a stream of audio from a file.
+
+    The audio is expected to be in the range (-1, 1).
+
+    Args:
+        in_file: Path to the input file.
+        chunk_length: Size of the chunks to read. If `None`, will iterate
+            whatever chunk size the underlying reader uses. Otherwise, samples
+            will be rechunked to the desired size.
+        sampling_rate: Sampling rate to resample the audio to. If `None`, will
+            use the sampling rate of the input audio.
+        reader: Reader to use. Can be either `ffmpeg` or `av`.
+
+    Returns:
+        Iterator over numpy arrays, with shape (n_channels, n_samples).
+    """
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in this system.")
             reader = "av"
         else:
-            return read_audio_ffmpeg(in_file)
+            sr = None if sampling_rate is None else (AudioProps.from_file_ffmpeg(in_file).sample_rate, sampling_rate)
+            return _resample_audio(read_audio_ffmpeg(in_file), chunk_length=chunk_length, sampling_rate=sr)
 
     if reader == "av":
-        return read_audio_av(in_file)
+        sr = None if sampling_rate is None else (AudioProps.from_file_av(in_file).sample_rate, sampling_rate)
+        return _resample_audio(read_audio_av(in_file), chunk_length=chunk_length, sampling_rate=sr)
 
     raise ValueError(f"Unknown reader {reader}")
 
 
 def write_audio(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     sample_rate: int,
     *,
-    writer: Writer = "ffmpeg",
+    writer: Writer = "av",
 ) -> None:
     """Function that writes a stream of audio to a file.
 
     Args:
         itr: Iterator of audio chunks.
         out_file: Path to the output file.
         sample_rate: Sample rate of the audio.
```

### Comparing `ml-starter-0.0.55/ml/utils/augmentation.py` & `ml-starter-0.0.56/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/caching.py` & `ml-starter-0.0.56/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/checkpoint.py` & `ml-starter-0.0.56/ml/utils/checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from ml.trainers.base import BaseTrainer
 from ml.utils.data import check_md5, check_sha256
 from ml.utils.device.auto import AutoDevice
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
+USER_AGENT = "ml-starter"
+
 T = TypeVar("T")
 
 
 def instantiate_config(config: str | Path | DictConfig | dict) -> Objects:
     """Builds the objects from the raw config.
 
     Args:
@@ -150,39 +152,69 @@
 
 def ensure_downloaded(
     url: str,
     *dnames: str,
     md5: str | None = None,
     sha256: str | None = None,
     is_tmp: bool = False,
+    use_tqdm: bool = True,
+    recheck_hash: bool = False,
 ) -> Path:
     """Ensures that a checkpoint URL has been downloaded.
 
     This basically just provides a nice way of organizing pre-trained models,
     by saving them to a consistent location.
 
     Args:
         url: The URL to download.
         dnames: The directory to download to (note that this is relative to the
             model directory). The final name should be the file name
         md5: The MD5 hash of the file, if known.
         sha256: The SHA256 hash of the file, if known.
         is_tmp: If set, use ``tmp/`` instead of ``get_model_dir()``
+        use_tqdm: Whether to use tqdm to show download progress.
+        recheck_hash: Whether to recheck the hash of the file if it already
+            exists.
 
     Returns:
         The path to the downloaded file.
     """
     assert len(dnames) >= 1, "Must provide at least 1 directory name"
     filepath = Path(tempfile.mkdtemp("models")) if is_tmp else get_model_dir()
     for dname in dnames:
         filepath = filepath / dname
     (root := filepath.parent).mkdir(parents=True, exist_ok=True)
-    if not filepath.exists() or not check_sha256(filepath, sha256) or not check_md5(filepath, md5):
-        download_url(url, root=root, filename=filepath.name, md5=md5)
+
+    def check_hashes() -> bool:
+        return (
+            filepath.is_file()
+            and check_sha256(filepath, sha256, use_tqdm=use_tqdm)
+            and check_md5(filepath, md5, use_tqdm=use_tqdm)
+        )
+
+    def download_file() -> None:
+        download_url(url, root=root, filename=filepath.name)
         assert filepath.is_file(), f"Failed to download {url} to {filepath}"
+        if not check_hashes():
+            filepath.unlink()
+            raise RuntimeError(f"Hashes for {url} do not match")
+
+    # If the file does not exist, download it and check the hashes.
+    if not filepath.exists():
+        download_file()
+
+    # By default, assume the downloaded file hash is correct.
+    if not recheck_hash:
+        return filepath
+
+    # Check the file hashes again, to ensure the file was not corrupted.
+    if not check_hashes():
+        filepath.unlink()
+        download_file()
+
     return filepath
 
 
 def get_state_dict_prefix(state_dict: Mapping[str, T], prefix: str) -> Mapping[str, T]:
     """Gets the state dict with a prefix removed from the keys.
 
     Args:
```

### Comparing `ml-starter-0.0.55/ml/utils/cli.py` & `ml-starter-0.0.56/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/colors.py` & `ml-starter-0.0.56/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/config.py` & `ml-starter-0.0.56/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/data.py` & `ml-starter-0.0.56/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/datetime.py` & `ml-starter-0.0.56/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/device/auto.py` & `ml-starter-0.0.56/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/device/base.py` & `ml-starter-0.0.56/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/device/cpu.py` & `ml-starter-0.0.56/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/device/gpu.py` & `ml-starter-0.0.56/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/device/metal.py` & `ml-starter-0.0.56/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/distributed.py` & `ml-starter-0.0.56/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/image.py` & `ml-starter-0.0.56/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/large_models.py` & `ml-starter-0.0.56/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/logging.py` & `ml-starter-0.0.56/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/meter.py` & `ml-starter-0.0.56/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/parallel.py` & `ml-starter-0.0.56/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/staging.py` & `ml-starter-0.0.56/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/timer.py` & `ml-starter-0.0.56/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/tokens.py` & `ml-starter-0.0.56/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/torch_distributed.py` & `ml-starter-0.0.56/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.55/ml/utils/video.py` & `ml-starter-0.0.56/ml/utils/video.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,53 +12,109 @@
 
     write_video(frame_iterator(), "/path/to/other/video.mp4")
 
 This just uses FFMPEG so it should be reasonably quick.
 """
 
 import asyncio
+import functools
 import re
 import shutil
 import warnings
 from dataclasses import dataclass
 from fractions import Fraction
 from pathlib import Path
 from typing import AsyncGenerator, Iterator, Literal
 
 import av
-import cv2
-import ffmpeg
-import matplotlib.animation as ani
-import matplotlib.pyplot as plt
 import numpy as np
+import torchvision.transforms.functional as F
 from torch import Tensor
 
 from ml.utils.image import as_uint8, standardize_image
 
 
+@functools.lru_cache()
+def ffmpeg_python_available() -> bool:
+    try:
+        import ffmpeg
+
+        assert ffmpeg is not None  # Silence unused import warning
+    except ImportError:
+        return False
+    else:
+        return True
+
+
+@functools.lru_cache()
+def mpl_available() -> bool:
+    try:
+        import matplotlib
+
+        assert matplotlib is not None  # Silence unused import warning
+    except ImportError:
+        return False
+    else:
+        return True
+
+
+@functools.lru_cache()
+def cv2_available() -> bool:
+    try:
+        import cv2
+
+        assert cv2 is not None  # Silence unused import warning
+    except ImportError:
+        return False
+    else:
+        return True
+
+
 @dataclass
 class VideoProps:
     frame_width: int
     frame_height: int
     frame_count: int
     fps: Fraction
 
     @classmethod
+    def from_file_av(cls, fpath: str | Path) -> "VideoProps":
+        container = av.open(str(fpath))
+        stream = container.streams.video[0]
+
+        return cls(
+            frame_width=stream.width,
+            frame_height=stream.height,
+            frame_count=stream.frames,
+            fps=Fraction(stream.average_rate),
+        )
+
+    @classmethod
     def from_file_opencv(cls, fpath: str | Path) -> "VideoProps":
+        try:
+            import cv2
+        except ImportError as e:
+            raise ImportError("Please install OpenCV to use this function: `pip install opencv-python`") from e
+
         cap = cv2.VideoCapture(str(fpath))
 
         return cls(
             frame_width=int(cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
             frame_height=int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT)),
             frame_count=int(cap.get(cv2.CAP_PROP_FRAME_COUNT)),
             fps=Fraction(cap.get(cv2.CAP_PROP_FPS)),
         )
 
     @classmethod
     def from_file_ffmpeg(cls, fpath: str | Path) -> "VideoProps":
+        try:
+            import ffmpeg
+        except ImportError as e:
+            raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+
         probe = ffmpeg.probe(str(fpath))
 
         for stream in probe["streams"]:
             if stream["codec_type"] == "video":
                 width, height, count = stream["width"], stream["height"], int(stream["nb_frames"])
                 fps_num, fps_denom = stream["r_frame_rate"].split("/")
                 return cls(
@@ -86,15 +142,15 @@
         Frames from the video as numpy arrays with shape (H, W, C)
     """
     container = av.open(str(in_file))
 
     for frame in container.decode(video=0):
         frame = frame.to_rgb().to_ndarray()
         if target_dims is not None:
-            frame = cv2.resize(frame, target_dims[::-1])
+            frame = F.resize(frame, target_dims[::-1])
         yield as_uint8(frame)
 
 
 def read_video_ffmpeg(
     in_file: str | Path,
     *,
     output_fmt: str = "rgb24",
@@ -106,14 +162,19 @@
         in_file: The input video to read
         output_fmt: The output image format
         channels: Number of output channels for each video frame
 
     Yields:
         Frames from the video as numpy arrays with shape (H, W, C)
     """
+    try:
+        import ffmpeg
+    except ImportError as e:
+        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+
     props = VideoProps.from_file_ffmpeg(in_file)
 
     stream = ffmpeg.input(str(in_file))
     stream = ffmpeg.output(stream, "pipe:", format="rawvideo", pix_fmt=output_fmt, r=float(props.fps))
     stream = ffmpeg.run_async(stream, pipe_stdout=True)
 
     while True:
@@ -142,14 +203,19 @@
         target_dims: (width, height) dimensions for images being loaded, with
             None meaning that the aspect ratio should be kept the same
 
     Yields:
         Frames from the video as numpy arrays with shape (H, W, C), along with
         the frame timestamps
     """
+    try:
+        import ffmpeg
+    except ImportError as e:
+        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+
     props = VideoProps.from_file_ffmpeg(in_file)
 
     def aspect_ratio(x: int, a: int, b: int) -> int:
         return (x * a + b - 1) // b
 
     vf: list[str] = []
     if target_dims is not None:
@@ -209,14 +275,19 @@
 
     Args:
         in_file: The input video to read
 
     Yields:
         Frames from the video as numpy arrays with shape (H, W, C)
     """
+    try:
+        import cv2
+    except ImportError as e:
+        raise ImportError("Please install OpenCV to use this function: `pip install opencv-python`") from e
+
     cap = cv2.VideoCapture(str(in_file))
 
     while True:
         ret, buffer = cap.read()
         if not ret:
             cap.release()
             return
@@ -238,14 +309,19 @@
         out_file: The path to the output file.
         keep_resolution: If set, don't change the image resolution, otherwise
             resize to a human-friendly resolution.
         fps: Frames per second for the video.
         codec: FourCC code specifying OpenCV video codec type. Examples are
             MPEG, MP4V, DIVX, AVC1, H236.
     """
+    try:
+        import cv2
+    except ImportError as e:
+        raise ImportError("Please install OpenCV to use this function: `pip install opencv-python`") from e
+
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
     first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
 
     fourcc = cv2.VideoWriter_fourcc(*codec)
     stream = cv2.VideoWriter(str(out_file), fourcc, fps if isinstance(fps, int) else round(fps), (width, height))
@@ -328,14 +404,19 @@
             resize to a human-friendly resolution.
         fps: Frames per second for the video.
         out_fps: Frames per second for the saved video.
         vcodec: The video codec to use for the output video
         input_fmt: The input image format
         output_fmt: The output image format
     """
+    try:
+        import ffmpeg
+    except ImportError as e:
+        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
     first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
 
     stream = ffmpeg.input("pipe:", format="rawvideo", pix_fmt=input_fmt, s=f"{width}x{height}", r=float(fps))
     stream = ffmpeg.output(stream, str(out_file), pix_fmt=output_fmt, vcodec=vcodec, r=float(out_fps))
@@ -376,14 +457,20 @@
         fps: Frames per second for the video.
         title: Title for the video metadata.
         comment: Comment for the video metadata.
         writer: The Matplotlib video writer to use (if you use the
             default one, make sure you have `ffmpeg` installed on your
             system).
     """
+    try:
+        import matplotlib.animation as ani
+        import matplotlib.pyplot as plt
+    except ImportError as e:
+        raise ImportError("Please install matplotlib to use this function: `pip install matplotlib`") from e
+
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
     first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
     fig, ax = plt.subplots(figsize=(width / dpi, height / dpi))
 
     # Ensures that there's no extra space around the image.
@@ -417,47 +504,78 @@
             mpl_writer.grab_frame()
 
 
 Reader = Literal["ffmpeg", "av", "opencv"]
 Writer = Literal["ffmpeg", "matplotlib", "av", "opencv"]
 
 
-def read_video(in_file: str | Path, *, reader: Reader = "ffmpeg") -> Iterator[np.ndarray]:
+def get_video_props(in_file: str | Path, *, reader: Reader = "av") -> VideoProps:
+    if reader == "ffmpeg":
+        if not shutil.which("ffmpeg"):
+            warnings.warn("FFMPEG is not available in this system.")
+            reader = "av"
+        elif not ffmpeg_python_available():
+            warnings.warn("FFMPEG Python is not installed; install with `pip install ffmpeg-python`")
+            reader = "av"
+        else:
+            return VideoProps.from_file_ffmpeg(in_file)
+
+    if reader == "opencv":
+        if not cv2_available():
+            warnings.warn("OpenCV is not installed; install with `pip install opencv-python`")
+            reader = "av"
+        else:
+            return VideoProps.from_file_opencv(in_file)
+
+    if reader == "av":
+        return VideoProps.from_file_av(in_file)
+
+    raise ValueError(f"Unknown reader {reader}")
+
+
+def read_video(in_file: str | Path, *, reader: Reader = "av") -> Iterator[np.ndarray]:
     """Function that reads a video from a file to a stream of Numpy arrays.
 
     Args:
         in_file: The path to the input file.
         reader: The video reader to use.
 
     Yields:
         The video frames as Numpy arrays.
     """
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in the system.")
             reader = "av"
+        elif not ffmpeg_python_available():
+            warnings.warn("FFMPEG Python is not installed; install with `pip install ffmpeg-python`")
+            reader = "av"
         else:
             return read_video_ffmpeg(in_file)
 
+    if reader == "opencv":
+        if not cv2_available():
+            warnings.warn("OpenCV is not installed; install with `pip install opencv-python`")
+            reader = "av"
+        else:
+            return read_video_opencv(in_file)
+
     if reader == "av":
         return read_video_av(in_file)
 
-    if reader == "opencv":
-        return read_video_opencv(in_file)
-
     raise ValueError(f"Invalid reader: {reader}")
 
 
 def write_video(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     *,
     fps: int | Fraction = 30,
     keep_resolution: bool = False,
-    writer: Writer = "ffmpeg",
+    writer: Writer = "av",
 ) -> None:
     """Function that writes an video from a stream of input tensors.
 
     Args:
         itr: The image iterator, yielding images with shape (H, W, C).
         out_file: The path to the output file.
         fps: Frames per second for the video.
@@ -468,28 +586,38 @@
     Raises:
         ValueError: If the writer is invalid.
     """
     if writer == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in the system.")
             writer = "av"
+        elif not ffmpeg_python_available():
+            warnings.warn("FFMPEG Python is not installed; install with `pip install ffmpeg-python`")
+            writer = "av"
         else:
             write_video_ffmpeg(itr, out_file, fps=fps, keep_resolution=keep_resolution)
             return
 
     if writer == "matplotlib":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in the system.")
             writer = "av"
+        elif not mpl_available():
+            warnings.warn("Matplotlib is not available in the system.")
+            writer = "av"
         else:
             write_video_matplotlib(itr, out_file, fps=fps, keep_resolution=keep_resolution)
             return
 
+    if writer == "opencv":
+        if not cv2_available():
+            warnings.warn("OpenCV is not installed; install with `pip install opencv-python`")
+            writer = "av"
+        else:
+            write_video_opencv(itr, out_file, fps=fps, keep_resolution=keep_resolution)
+            return
+
     if writer == "av":
         write_video_av(itr, out_file, fps=fps, keep_resolution=keep_resolution)
         return
 
-    if writer == "opencv":
-        write_video_opencv(itr, out_file, fps=fps, keep_resolution=keep_resolution)
-        return
-
     raise ValueError(f"Invalid writer: {writer}")
```

### Comparing `ml-starter-0.0.55/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.56/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.55
+Version: 0.0.56
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.55/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.56/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 ml/models/parallel.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adamw.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
 ml/optimizers/common.py
+ml/optimizers/lion.py
 ml/optimizers/sgd.py
 ml/optimizers/shampoo.py
 ml/optimizers/types.py
 ml/scripts/__init__.py
 ml/scripts/cli.py
 ml/scripts/launch.py
 ml/scripts/resolve.py
@@ -129,12 +130,14 @@
 ml/utils/video.py
 ml/utils/device/__init__.py
 ml/utils/device/auto.py
 ml/utils/device/base.py
 ml/utils/device/cpu.py
 ml/utils/device/gpu.py
 ml/utils/device/metal.py
+ml/utils/triton/__init__.py
+ml/utils/triton/lion.py
 ml_starter.egg-info/PKG-INFO
 ml_starter.egg-info/SOURCES.txt
 ml_starter.egg-info/dependency_links.txt
 ml_starter.egg-info/requires.txt
 ml_starter.egg-info/top_level.txt
```

### Comparing `ml-starter-0.0.55/pyproject.toml` & `ml-starter-0.0.56/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 testpaths = ["tests"]
 
 markers = [
     "slow: Marks test as being slow",
     "has_gpu: Marks test as requiring a GPU to run",
     "multi_gpu: Marks tests as requiring multiple GPUs to run",
     "has_mps: Marks test as requiring an MPS device to run",
+    "has_triton: Marks test as requiring Triton is installed to run",
 ]
 
 [tool.mypy]
 
 pretty = true
 show_column_numbers = true
 show_error_context = true
@@ -40,15 +41,17 @@
 [[tool.mypy.overrides]]
 
 module = [
     "av.*",
     "cv2.*",
     "ffmpeg.*",
     "matplotlib.*",
+    "torchaudio.*",
     "torchvision.*",
+    "triton.*",
 ]
 
 ignore_missing_imports = true
 
 [tool.isort]
 
 profile = "black"
```

### Comparing `ml-starter-0.0.55/setup.py` & `ml-starter-0.0.56/setup.py`

 * *Files identical despite different names*

