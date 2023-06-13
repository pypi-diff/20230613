# Comparing `tmp/glow-0.12.5.tar.gz` & `tmp/glow-0.12.6.tar.gz`

## Comparing `glow-0.12.5.tar` & `glow-0.12.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.5/examples/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.5/examples/cifar10.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.5/examples/gan.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/__init__.py
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/cli.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/cli.pyi
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/distributed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/py.typed
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/api/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/api/config.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/api/exporting.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/__init__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_coro.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_import_hook.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_more.py
--rw-r--r--   0        0        0    15170 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_parallel.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_parallel.pyi
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_patch_len.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_patch_print.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_patch_scipy.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_profile.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_profile.pyi
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_reduction.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_repr.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_sizeof.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_thread_quota.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_uuid.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/debug.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/__init__.py
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/cache.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/cache.pyi
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/concurrency.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/concurrency.pyi
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/reusable.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/util.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/io/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/io/_sound.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/io/_svg.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/__init__.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/base.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/confusion.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/raw.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/__init__.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/_loader.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/_sampler.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/_trainer.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/amp.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/driver.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/functional.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/optimizers.py
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/plot.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/proto.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/util.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/__init__.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/aggregates.py
--rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/context.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/convnets.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/lazy.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/simple.py
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/transformers.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/util.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/vision.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/__init__.py
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/classes.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/core.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/functional/__init__.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/functional/core.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/functional/numba.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.5/test/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.5/test/run_metrics.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_api.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_batch.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_buffered.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_cli.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_iter.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_loader.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_shm.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_thread_pool.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_timed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_timer.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_uuid.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.5/LICENSE
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.5/README.md
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 glow-0.12.5/pyproject.toml
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 glow-0.12.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.6/examples/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.6/examples/cifar10.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.6/examples/gan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/__init__.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/cli.pyi
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/distributed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/api/exporting.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/__init__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_coro.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_import_hook.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_more.py
+-rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_parallel.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_parallel.pyi
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_patch_print.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_patch_scipy.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_profile.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_profile.pyi
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_reduction.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_repr.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_sizeof.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_thread_quota.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/_uuid.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/debug.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/wrap/__init__.py
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/wrap/cache.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/wrap/cache.pyi
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/wrap/concurrency.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/wrap/reusable.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/core/wrap/util.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/metrics/__init__.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/metrics/base.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/metrics/confusion.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/metrics/raw.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/__init__.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/_loader.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/_sampler.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/_trainer.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/amp.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/driver.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/functional.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/optimizers.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/plot.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/proto.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/util.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/__init__.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/aggregates.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/context.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/convnets.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/lazy.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/simple.py
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/transformers.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/util.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/nn/modules/vision.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/transforms/__init__.py
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/transforms/classes.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/transforms/core.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/transforms/functional/core.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.6/src/glow/transforms/functional/numba.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.6/test/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.6/test/run_metrics.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_buffered.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_iter.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_loader.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_shm.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.6/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.6/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.6/README.md
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 glow-0.12.6/pyproject.toml
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 glow-0.12.6/PKG-INFO
```

### Comparing `glow-0.12.5/examples/cifar10.py` & `glow-0.12.6/examples/cifar10.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/cli.py` & `glow-0.12.6/src/glow/cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/cli.pyi` & `glow-0.12.6/src/glow/cli.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/distributed.py` & `glow-0.12.6/src/glow/distributed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/api/config.py` & `glow-0.12.6/src/glow/api/config.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/api/exporting.py` & `glow-0.12.6/src/glow/api/exporting.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/__init__.py` & `glow-0.12.6/src/glow/core/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from . import _patch_len, _patch_print, _patch_scipy
 from ._coro import as_actor, coroutine, summary
-from ._more import as_iter, chunked, eat, ichunked, roundrobin, windowed
-from ._parallel import buffered, map_n, starmap_n
+from ._more import as_iter, chunked, eat, ichunked, ilen, roundrobin, windowed
+from ._parallel import buffered, map_n, map_n_dict, starmap_n
 from ._profile import memprof, time_this, timer
 from ._repr import countable, mangle, repr_as_obj, si, si_bin
 from ._sizeof import sizeof
 from ._uuid import Uid
 from .debug import lock_seed, trace, trace_module, whereami
 from .wrap import (Reusable, call_once, memoize, shared_call, streaming,
                    threadlocal)
 
 __all__ = [
     'Reusable', 'Uid', 'as_actor', 'as_iter', 'buffered', 'call_once',
-    'chunked', 'coroutine', 'countable', 'eat', 'ichunked', 'lock_seed',
-    'mangle', 'map_n', 'memoize', 'memprof', 'repr_as_obj', 'roundrobin',
-    'shared_call', 'si', 'si_bin', 'sizeof', 'starmap_n', 'streaming',
-    'summary', 'threadlocal', 'time_this', 'timer', 'trace', 'trace_module',
-    'whereami', 'windowed'
+    'chunked', 'coroutine', 'countable', 'eat', 'ichunked', 'ilen',
+    'lock_seed', 'mangle', 'map_n', 'map_n_dict', 'memoize', 'memprof',
+    'repr_as_obj', 'roundrobin', 'shared_call', 'si', 'si_bin', 'sizeof',
+    'starmap_n', 'streaming', 'summary', 'threadlocal', 'time_this', 'timer',
+    'trace', 'trace_module', 'whereami', 'windowed'
 ]
 
 _patch_print.apply()
 _patch_len.apply()
 _patch_scipy.apply()
```

### Comparing `glow-0.12.5/src/glow/core/_coro.py` & `glow-0.12.6/src/glow/core/_coro.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_import_hook.py` & `glow-0.12.6/src/glow/core/_import_hook.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_more.py` & `glow-0.12.6/src/glow/core/_more.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
-__all__ = ['as_iter', 'chunked', 'eat', 'ichunked', 'roundrobin', 'windowed']
+__all__ = [
+    'as_iter', 'chunked', 'eat', 'ichunked', 'ilen', 'roundrobin', 'windowed'
+]
 
 import threading
 from collections import deque
 from collections.abc import Iterable, Iterator, Mapping, Sequence, Sized
 from functools import partial
-from itertools import chain, cycle, islice, repeat
+from itertools import chain, count, cycle, islice, repeat
 from typing import Protocol, TypeVar, overload
 
 _T = TypeVar('_T')
 _T_co = TypeVar('_T_co', covariant=True)
 
 
 class SupportsSlice(Sized, Protocol[_T_co]):
@@ -84,14 +86,15 @@
     return map(s.__getitem__, slices)
 
 
 def _chunked(it: Iterable[_T], size: int) -> Iterator[tuple[_T, ...]]:
     if size == 1:  # Trivial case
         return zip(it)
 
+    # TODO: python 3.12 - `itertools.batched(it, size)`
     fetch_chunk = partial(islice, iter(it), size)
     chunks = iter(fetch_chunk, None)
     return iter(map(tuple, chunks).__next__, ())  # type: ignore[arg-type]
 
 
 # ---------------------------------------------------------------------------
 
@@ -186,20 +189,31 @@
         # Advance and fill internal cache, expand tail with items from body
         tail += body
 
 
 # ----------------------------------------------------------------------------
 
 
+def ilen(iterable: Iterable) -> int:
+    """Return number of items in *iterable*.
+
+    This consumes iterable, so handle with care.
+    See `more_itertools.ilen`.
+    """
+    counter = count()
+    deque(zip(iterable, counter), maxlen=0)
+    return next(counter)
+
+
 def eat(iterable: Iterable, daemon: bool = False) -> None:
     """Consume iterable, daemonize if needed (move to background thread)"""
     if daemon:
         threading.Thread(target=deque, args=(iterable, 0), daemon=True).start()
     else:
-        deque(iterable, 0)
+        deque(iterable, 0)  # Same as `more_itertools.consume(..., n=None)`
 
 
 def roundrobin(*iterables: Iterable[_T]) -> Iterator[_T]:
     """roundrobin('ABC', 'D', 'EF') --> A D E B F C"""
     iters = cycle(iter(it) for it in iterables)
     for pending in range(len(iterables) - 1, -1, -1):
         yield from map(next, iters)
```

### Comparing `glow-0.12.5/src/glow/core/_parallel.py` & `glow-0.12.6/src/glow/core/_parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
-__all__ = ['buffered', 'map_n', 'starmap_n']
+__all__ = ['buffered', 'map_n', 'map_n_dict', 'starmap_n']
 
 import atexit
 import enum
 import os
 import signal
 import sys
 import warnings
 import weakref
-from collections.abc import Callable, Iterable, Iterator, Sized
+from collections.abc import Callable, Iterable, Iterator, Mapping, Sized
 from concurrent.futures import Executor, Future
 from concurrent.futures import TimeoutError as _TimeoutError
 from contextlib import ExitStack, contextmanager
 from cProfile import Profile
 from functools import partial
 from itertools import chain, islice, starmap
 from multiprocessing.managers import BaseManager
@@ -27,19 +27,21 @@
 import loky
 
 try:
     import psutil
 except ImportError:
     psutil = None
 
-from ._more import chunked
+from ._more import chunked, ilen
 from ._reduction import move_to_shmem, reducers
 from ._thread_quota import ThreadQuota
 
 _T = TypeVar('_T')
+_T_ctr = TypeVar('_T_ctr', contravariant=True)
+_K = TypeVar('_K')
 _F = TypeVar('_F', bound=Future)
 
 _NUM_CPUS = os.cpu_count() or 0
 _NUM_CPUS = min(_NUM_CPUS, int(os.getenv('GLOW_CPUS', _NUM_CPUS)))
 _IDLE_WORKER_TIMEOUT = 10
 _GRANULAR_SCHEDULING = False  # TODO: investigate whether this improves load
 
@@ -104,26 +106,27 @@
 
 _PATIENCE = 0.01
 
 
 def _retry_call(fn: Callable[..., _T], *exc: type[BaseException]) -> _T:
     # See issues
     # https://bugs.python.org/issue29971
+    # https://github.com/python/cpython/issues/74157
     # https://github.com/dask/dask/pull/2144#issuecomment-290556996
     # https://github.com/dask/dask/pull/2144/files
     while True:
         try:
             return fn(timeout=_PATIENCE)
         except exc:
             sleep(0)  # Force switch to another thread to proceed
 
 
 if sys.platform == 'win32':
 
-    def _result(f: Future[_T]) -> _T:
+    def _result(f: Future[_T], /) -> _T:
         return _retry_call(f.result, _TimeoutError)
 else:
     _result = Future.result
 
 
 def _result_or_cancel(f: Future[_T]) -> _T:
     try:
@@ -358,21 +361,23 @@
 
 def _unwrap(s: ExitStack, fs: Iterable[Future[_T]], qsize: int | None,
             order: bool) -> Iterator[_T]:
     q = SimpleQueue[Future[_T]]()
 
     # If `order`, then `q` has "PENDING"/"RUNNING"/"DONE" tasks,
     # otherwise it only has "DONE" tasks.
-    q_put = q.put if order else methodcaller('add_done_callback', q.put)
+    # FIXME: order=False -> random freezes (in q.get -> Empty)
+    q_put = cast(Callable[[Future[_T]], None],
+                 q.put if order else methodcaller('add_done_callback', q.put))
 
     # On each `next()` schedules new task
-    fs_scheduler = map(q_put, fs)  # type: ignore[call-overload]
+    fs_scheduler = map(q_put, fs)
     try:
         # Fetch up to `qsize` tasks to pre-fill `q`
-        qsize = sum(1 for _ in islice(fs_scheduler, qsize))
+        qsize = ilen(islice(fs_scheduler, qsize))
 
     except BaseException:
         # Unwind stack here on an error
         s.close()
         raise
 
     else:
@@ -494,7 +499,29 @@
         func,
         zip(*iterables),
         max_workers=max_workers,
         prefetch=prefetch,
         mp=mp,
         chunksize=chunksize,
         order=order)
+
+
+def map_n_dict(func: Callable[[_T_ctr], _T],
+               obj: Mapping[_K, _T_ctr],
+               /,
+               *,
+               max_workers: int | None = None,
+               prefetch: int | None = 2,
+               mp: bool = False,
+               chunksize: int | None = None) -> dict[_K, _T]:
+    """
+    Apply `func` to each value in a mapping in parallel way.
+    For extra options, see starmap_n, which is used under hood.
+    """
+    iter_values = map_n(
+        func,
+        obj.values(),
+        max_workers=max_workers,
+        prefetch=prefetch,
+        mp=mp,
+        chunksize=chunksize)
+    return dict(zip(obj.keys(), iter_values))
```

### Comparing `glow-0.12.5/src/glow/core/_parallel.pyi` & `glow-0.12.6/src/glow/core/_parallel.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from collections.abc import Callable, Iterable, Iterator
+from collections.abc import Callable, Iterable, Iterator, Mapping
 from concurrent.futures import Executor
 from typing import Generic, Protocol, TypeVar, overload
 
 _T = TypeVar('_T')
 _T1_ctr = TypeVar('_T1_ctr', contravariant=True)
 _T2_ctr = TypeVar('_T2_ctr', contravariant=True)
 _T3_ctr = TypeVar('_T3_ctr', contravariant=True)
+_K_co = TypeVar('_K_co', covariant=True)
 _R_co = TypeVar('_R_co', covariant=True)
 
 
 class _Callable1(Generic[_T1_ctr, _R_co], Protocol):
     def __call__(self, __1: _T1_ctr, /) -> _R_co:
         ...
 
@@ -105,7 +106,18 @@
           *__iters: Iterable,
           max_workers: int | None = ...,
           prefetch: int | None = ...,
           mp: bool = ...,
           chunksize: int | None = ...,
           order: bool = ...) -> Iterator[_R_co]:
     ...
+
+
+def map_n_dict(func: Callable[[_T1_ctr], _R_co],
+               obj: Mapping[_K_co, _T1_ctr],
+               /,
+               *,
+               max_workers: int | None = None,
+               prefetch: int | None = 2,
+               mp: bool = False,
+               chunksize: int | None = None) -> dict[_K_co, _R_co]:
+    ...
```

### Comparing `glow-0.12.5/src/glow/core/_patch_len.py` & `glow-0.12.6/src/glow/core/_patch_len.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_patch_print.py` & `glow-0.12.6/src/glow/core/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_patch_scipy.py` & `glow-0.12.6/src/glow/core/_patch_scipy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_profile.py` & `glow-0.12.6/src/glow/core/_profile.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_profile.pyi` & `glow-0.12.6/src/glow/core/_profile.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_reduction.py` & `glow-0.12.6/src/glow/core/_reduction.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_repr.py` & `glow-0.12.6/src/glow/core/_repr.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_sizeof.py` & `glow-0.12.6/src/glow/core/_sizeof.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_thread_quota.py` & `glow-0.12.6/src/glow/core/_thread_quota.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/_uuid.py` & `glow-0.12.6/src/glow/core/_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/debug.py` & `glow-0.12.6/src/glow/core/debug.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/wrap/cache.py` & `glow-0.12.6/src/glow/core/wrap/cache.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/wrap/cache.pyi` & `glow-0.12.6/src/glow/core/wrap/cache.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/wrap/concurrency.py` & `glow-0.12.6/src/glow/core/wrap/concurrency.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/wrap/concurrency.pyi` & `glow-0.12.6/src/glow/core/wrap/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/wrap/reusable.py` & `glow-0.12.6/src/glow/core/wrap/reusable.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/core/wrap/util.py` & `glow-0.12.6/src/glow/core/wrap/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/io/_sound.py` & `glow-0.12.6/src/glow/io/_sound.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/io/_svg.py` & `glow-0.12.6/src/glow/io/_svg.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/metrics/__init__.py` & `glow-0.12.6/src/glow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/metrics/base.py` & `glow-0.12.6/src/glow/metrics/base.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/metrics/confusion.py` & `glow-0.12.6/src/glow/metrics/confusion.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/metrics/raw.py` & `glow-0.12.6/src/glow/metrics/raw.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/__init__.py` & `glow-0.12.6/src/glow/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/_loader.py` & `glow-0.12.6/src/glow/nn/_loader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 __all__ = ['get_loader']
 
 import os
+import re
 import warnings
-from collections.abc import Iterator, Sequence, Sized
+from collections.abc import Callable, Iterator, Mapping, Sequence, Sized
 from dataclasses import dataclass, replace
+from functools import partial
 from itertools import islice
 from typing import Any, Protocol
 
+import numpy as np
 import torch
 from torch.utils.data import (Dataset, IterableDataset, RandomSampler, Sampler,
                               SequentialSampler)
 from torch.utils.data._utils import worker as torch_worker
 
 from .. import buffered, chunked, map_n, roundrobin
 from ..core._parallel import _get_executor, max_cpu_count
@@ -63,66 +66,71 @@
         return _PinningLoader(self) if torch.cuda.is_available() else self
 
 
 # --------------------------------- batching ---------------------------------
 
 
 class _CollateFn(Protocol):
-    def __call__(self, __items: Sequence) -> Any:
+    def __call__(self, __items: tuple) -> Any:
         ...
 
 
-def default_collate(batch: Sequence[tuple]) -> Any:
-    return *(torch.stack([torch.as_tensor(item) for item in row])
-             for row in zip(*batch)),
-
-
 @dataclass(frozen=True)
 class _BatchedLoader(_PinnableLoader):
     base: _Loader
     batch_size: int
     collate_fn: _CollateFn
     drop_last: bool
+    workers: int
 
     def __iter__(self) -> Iterator:
         it = iter(self.base)
 
         if self.drop_last:
             total = len(self) * self.batch_size
             it = islice(it, total)
 
         batches = chunked(it, self.batch_size)
-        return map(self.collate_fn, batches)
+        return map_n(self.collate_fn, batches, max_workers=self.workers)
 
     def __len__(self) -> int:
         len_ = len(self.base)
 
         if self.drop_last:
             return len_ // self.batch_size
 
         return len(range(0, len_, self.batch_size))
 
 
 class _BatchableLoader(_PinnableLoader):
     def batch(self,
               batch_size: int,
-              collate_fn: _CollateFn = default_collate,
-              drop_last: bool = False) -> _BatchedLoader:
+              collate_fn: _CollateFn | None = None,
+              drop_last: bool = False,
+              daemon: bool = False) -> _BatchedLoader:
         """
         Groups data into batches.
 
         Parameters:
         - batch_size - How many samples per batch to load
         - collate_fn - Merges a list of samples to form a mini-batch of
           Tensor(s).
         - drop_last - Set to `True` to drop the last incomplete batch,
           if size of underlying loader is not divisible by the batch size.
           Otherwise the last batch can be smaller than others.
+        - daemon - Set to do batching in background thread.
         """
-        return _BatchedLoader(self, batch_size, collate_fn, drop_last)
+        if collate_fn is None:
+            collate_fn = collate
+        # TODO: return _BatchedLoader(
+        #   replace(self, finalize=None),
+        #   batch_size, collate_fn, drop_last,
+        # )
+        return _BatchedLoader(self, batch_size, collate_fn, drop_last,
+                              int(daemon))
 
     def shuffle(self,
                 sampler: Sampler | SamplerLike | None) -> _BatchableLoader:
         """
         Reshuffle data at every epoch.
 
         Parameters:
@@ -143,16 +151,20 @@
     def __iter__(self) -> Iterator:
         return map(self.dataset.__getitem__, self.sampler)
 
     def __len__(self) -> int:
         assert isinstance(self.sampler, Sized)
         return len(self.sampler)
 
-    def shuffle(self, sampler: Sampler | SamplerLike | None) -> _MapLoader:
-        if sampler is None:
+    def shuffle(self,
+                sampler: Sampler | SamplerLike | bool | None) -> _MapLoader:
+        if not sampler:
+            return self
+
+        if sampler is True:
             assert isinstance(self.dataset, Sized)
             sampler = RandomSampler(self.dataset)
 
         return replace(self, sampler=DdpSampler(sampler))
 
 
 @dataclass(frozen=True)
@@ -271,7 +283,111 @@
             raise TypeError("dataset should be sized when it's not iterable")
 
         sampler = SequentialSampler(dataset)
 
         if not max_workers:
             return _MapLoader(dataset, DdpSampler(sampler))
         return _MapMultiLoader(dataset, DdpSampler(sampler), max_workers, mp)
+
+
+# ---------------- convert & collate. forked from pytorch 2.0 ----------------
+
+# TODO: split `collate` to `convert` (within worker) + `collate` (in main)
+# TODO: i.e. "Loader".tensors [alters workers] .batch() [adds collation]
+
+
+def convert(x):  # noqa: PLR0911
+    tp = type(x)
+    if isinstance(x, torch.Tensor):
+        return x
+
+    if tp.__module__ == 'numpy' and not isinstance(x, np.str_ | np.bytes_):
+        if (isinstance(x, np.ndarray)
+                and _NP_STR_DTYPE_PATTERN.search(x.dtype.str)):
+            return x
+        return torch.as_tensor(x)
+
+    if isinstance(x, Mapping):
+        return _apply_type(tp, {k: convert(v) for k, v in x.items()})
+
+    if isinstance(x, Sequence) and not isinstance(x, str | bytes):
+        list_ = [convert(xx) for xx in x]
+
+        if isinstance(x, tuple) and hasattr(x, '_fields'):  # namedtuple
+            return tp(*list_)
+        return _apply_type(tp, list_)
+
+    return x
+
+
+def collate(batch):
+    x0 = batch[0]
+    tp = type(x0)
+
+    if _HINT is not None:  # Fast alternative to functools.singledispatch
+        fn = _HINT.get(tp) or next(
+            (fn for tp_, fn in _HINT.items() if isinstance(x0, tp_)), None)
+        if fn is not None:
+            return fn(batch)
+
+    if isinstance(x0, Mapping):
+        return _apply_type(tp, {k: collate([x[k] for x in batch]) for k in x0})
+
+    if isinstance(x0, Sequence):
+        assert len({len(x) for x in batch}) <= 1  # py3.10+: zip(strict=True)
+        list_ = [collate(samples) for samples in zip(*batch)]
+
+        if isinstance(x0, tuple) and hasattr(x0, '_fields'):  # namedtuple
+            return tp(*list_)
+        return _apply_type(tp, list_)
+
+    raise TypeError(_COLLATE_ERROR_MSG.format(tp))
+
+
+def _apply_type(tp, x):
+    try:
+        return tp(x)
+    except TypeError:
+        return x
+
+
+def _collate_tensor(batch: Sequence[torch.Tensor]):
+    x = batch[0]
+    out = None
+    if torch_worker.get_worker_info() is not None:
+        # If we're in a background process, concatenate directly into a
+        # shared memory tensor to avoid an extra copy
+        numel = sum(x.numel() for x in batch)
+        storage = x._typed_storage()._new_shared(numel, device=x.device)
+        out = x.new(storage).resize_(len(batch), *x.shape)
+
+    return torch.stack([*batch], out=out)
+
+
+def _collate_ndarray(batch: Sequence[np.ndarray]):
+    x = batch[0]
+    if _NP_STR_DTYPE_PATTERN.search(x.dtype.str):
+        raise TypeError(_COLLATE_ERROR_MSG.format(x.dtype))
+
+    return collate([torch.as_tensor(x) for x in batch])
+
+
+def _nop(batch):
+    return batch
+
+
+_HINT: dict[type | tuple[type, ...], Callable] = {
+    torch.Tensor: _collate_tensor,
+    np.ndarray: _collate_ndarray,  # For both ndarray and memmap
+    # Skip strings
+    bytes: _nop,
+    str: _nop,
+    # Tensorify scalars
+    (np.bool_, np.number, np.object_): torch.as_tensor,  # py3.10: UnionType
+    float: partial(torch.tensor, dtype=torch.float64),
+    int: torch.tensor,
+}
+
+_NP_STR_DTYPE_PATTERN = re.compile('[SOUa]')
+_COLLATE_ERROR_MSG = (
+    'default_collate: batch must contain tensors, numpy arrays, numbers, '
+    'dicts or lists; found {}')
```

### Comparing `glow-0.12.5/src/glow/nn/_sampler.py` & `glow-0.12.6/src/glow/nn/_sampler.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/_trainer.py` & `glow-0.12.6/src/glow/nn/_trainer.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/amp.py` & `glow-0.12.6/src/glow/nn/amp.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/driver.py` & `glow-0.12.6/src/glow/nn/driver.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/functional.py` & `glow-0.12.6/src/glow/nn/functional.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/optimizers.py` & `glow-0.12.6/src/glow/nn/optimizers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/plot.py` & `glow-0.12.6/src/glow/nn/plot.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/proto.py` & `glow-0.12.6/src/glow/nn/proto.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/util.py` & `glow-0.12.6/src/glow/nn/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/__init__.py` & `glow-0.12.6/src/glow/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/aggregates.py` & `glow-0.12.6/src/glow/nn/modules/aggregates.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/context.py` & `glow-0.12.6/src/glow/nn/modules/context.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/convnets.py` & `glow-0.12.6/src/glow/nn/modules/convnets.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/lazy.py` & `glow-0.12.6/src/glow/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/simple.py` & `glow-0.12.6/src/glow/nn/modules/simple.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/transformers.py` & `glow-0.12.6/src/glow/nn/modules/transformers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/util.py` & `glow-0.12.6/src/glow/nn/modules/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/nn/modules/vision.py` & `glow-0.12.6/src/glow/nn/modules/vision.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/transforms/__init__.py` & `glow-0.12.6/src/glow/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/transforms/classes.py` & `glow-0.12.6/src/glow/transforms/classes.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/transforms/core.py` & `glow-0.12.6/src/glow/transforms/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/transforms/functional/core.py` & `glow-0.12.6/src/glow/transforms/functional/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/src/glow/transforms/functional/numba.py` & `glow-0.12.6/src/glow/transforms/functional/numba.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/run_metrics.py` & `glow-0.12.6/test/run_metrics.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_api.py` & `glow-0.12.6/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_batch.py` & `glow-0.12.6/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_buffered.py` & `glow-0.12.6/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_cli.py` & `glow-0.12.6/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_iter.py` & `glow-0.12.6/test/test_iter.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_shm.py` & `glow-0.12.6/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_thread_pool.py` & `glow-0.12.6/test/test_thread_pool.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_timed.py` & `glow-0.12.6/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/test/test_uuid.py` & `glow-0.12.6/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/LICENSE` & `glow-0.12.6/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/README.md` & `glow-0.12.6/README.md`

 * *Files identical despite different names*

### Comparing `glow-0.12.5/pyproject.toml` & `glow-0.12.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "glow"
-version = "0.12.5"
+version = "0.12.6"
 description = "Functional Python tools with a PyTorch flavour"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `glow-0.12.5/PKG-INFO` & `glow-0.12.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glow
-Version: 0.12.5
+Version: 0.12.6
 Summary: Functional Python tools with a PyTorch flavour
 Project-URL: homepage, https://github.com/arquolo/glow
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Paul Maevskikh
```

