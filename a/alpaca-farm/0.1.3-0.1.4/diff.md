# Comparing `tmp/alpaca_farm-0.1.3.tar.gz` & `tmp/alpaca_farm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_farm-0.1.3.tar", last modified: Sun Jun 11 21:49:21 2023, max compression
+gzip compressed data, was "alpaca_farm-0.1.4.tar", last modified: Mon Jun 12 23:54:25 2023, max compression
```

## Comparing `alpaca_farm-0.1.3.tar` & `alpaca_farm-0.1.4.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.996693 alpaca_farm-0.1.3/
--rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.3/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.3/MANIFEST.in
--rw-r--r--   0 xuechenli   (501) staff       (20)    17050 2023-06-11 21:49:21.996528 alpaca_farm-0.1.3/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)    16449 2023-06-11 21:47:42.000000 alpaca_farm-0.1.3/README.md
--rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-11 21:49:21.996728 alpaca_farm-0.1.3/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)     2524 2023-06-11 20:30:56.000000 alpaca_farm-0.1.3/setup.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.978016 alpaca_farm-0.1.3/src/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.982857 alpaca_farm-0.1.3/src/alpaca_farm/
--rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-11 21:49:04.000000 alpaca_farm-0.1.3/src/alpaca_farm/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/accelerate_patch.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.985257 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/
--rw-r--r--   0 xuechenli   (501) staff       (20)      634 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1894 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/analysis.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.978375 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.990127 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6969 2023-06-11 02:31:44.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.992740 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      481 2023-06-11 02:31:44.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.992977 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/test/
--rw-r--r--   0 xuechenli   (501) staff       (20)      426 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     4951 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/decoders.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4762 2023-06-11 03:32:13.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/eval.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    29607 2023-06-10 06:19:54.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/pairwise_annotators.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11403 2023-06-10 06:21:13.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-11 04:26:11.000000 alpaca_farm-0.1.3/src/alpaca_farm/common.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/constants.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1369 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/data_postprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    18874 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/data_preprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4147 2023-06-11 21:47:42.000000 alpaca_farm-0.1.3/src/alpaca_farm/data_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/distributed_utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.993798 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/apex_patch.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/tensor_ops.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.994611 alpaca_farm-0.1.3/src/alpaca_farm/inference/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/inference/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.3/src/alpaca_farm/inference/decode.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/inference/score.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/logging.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.995137 alpaca_farm-0.1.3/src/alpaca_farm/models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.3/src/alpaca_farm/models/reward_model.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/models/rl_models.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11532 2023-06-10 06:21:02.000000 alpaca_farm-0.1.3/src/alpaca_farm/openai_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/reward_modeling_trainer.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.995889 alpaca_farm-0.1.3/src/alpaca_farm/rl/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/kl_controller.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    22881 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13765 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/rl_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/trainer_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/types.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     6141 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.983733 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)    17050 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     4266 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      295 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/top_level.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.996332 alpaca_farm-0.1.3/tests/
--rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/tests/test_flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/tests/test_flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/tests/test_torch_ops.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.426278 alpaca_farm-0.1.4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.4/LICENSE
+-rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.4/MANIFEST.in
+-rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-12 23:54:25.426096 alpaca_farm-0.1.4/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16695 2023-06-12 23:53:35.000000 alpaca_farm-0.1.4/README.md
+-rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-12 23:54:25.426314 alpaca_farm-0.1.4/setup.cfg
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2524 2023-06-11 20:30:56.000000 alpaca_farm-0.1.4/setup.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.405768 alpaca_farm-0.1.4/src/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.411159 alpaca_farm-0.1.4/src/alpaca_farm/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-12 23:53:35.000000 alpaca_farm-0.1.4/src/alpaca_farm/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/accelerate_patch.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.413518 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      635 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1894 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/analysis.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.406126 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.421022 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6969 2023-06-11 02:31:44.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.421504 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      481 2023-06-11 02:31:44.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.421777 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/test/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      426 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4951 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/decoders.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4763 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/eval.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    28834 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/pairwise_annotators.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11404 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-12 18:21:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/common.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/constants.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1565 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/data_postprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21184 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/data_preprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4527 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/data_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/distributed_utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.422832 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/apex_patch.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/flash_models/tensor_ops.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.423385 alpaca_farm-0.1.4/src/alpaca_farm/inference/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/inference/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.4/src/alpaca_farm/inference/decode.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/inference/score.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/logging.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.424015 alpaca_farm-0.1.4/src/alpaca_farm/models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.4/src/alpaca_farm/models/reward_model.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/models/rl_models.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11542 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/openai_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/reward_modeling_trainer.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.425280 alpaca_farm-0.1.4/src/alpaca_farm/rl/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/kl_controller.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    22890 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/quark_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7932 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/quark_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13749 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/rl/rl_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/torch_ops.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/src/alpaca_farm/trainer_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-06-11 22:43:54.000000 alpaca_farm-0.1.4/src/alpaca_farm/types.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6767 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/src/alpaca_farm/utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.411897 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    17296 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4356 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/SOURCES.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/dependency_links.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      295 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/requires.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-12 23:54:25.000000 alpaca_farm-0.1.4/src/alpaca_farm.egg-info/top_level.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-12 23:54:25.425848 alpaca_farm-0.1.4/tests/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/tests/test_flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/tests/test_flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.4/tests/test_torch_ops.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      581 2023-06-12 23:52:33.000000 alpaca_farm-0.1.4/tests/test_utils.py
```

### Comparing `alpaca_farm-0.1.3/LICENSE` & `alpaca_farm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/PKG-INFO` & `alpaca_farm-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_farm
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -249,15 +249,15 @@
 
 ### RLHF with PPO
 
 To replicate our RLHF PPO model trained with simulated reward model in the paper, run
 
 ```bash
 bash examples/scripts/rlhf_ppo.sh \
-  <your_output_dir> \
+  <your_output_dir_for_ppo> \
   <your_wandb_run_name> \
   <your_output_dir_for_reward_model> \
   <your_output_dir_for_sft10k> \
   <kl_coef>
 ```
 
 `<your_output_dir_for_reward_model>` should point to either simulated reward model or human reward model trained
@@ -312,14 +312,27 @@
 bash examples/scripts/expiter.sh \
   <your_output_dir_for_expiter> \
   <your_wandb_run_name> \
   <your_output_dir_for_sft10k> \
   <your_output_dir_for_expiter_data>
 ```
 
+### Quark
+
+To replicate our Quark results for the AlpacaFarm evaluation suite, run
+
+```bash
+bash examples/scripts/rlhf_quark.sh \
+  <your_output_dir_for_quark> \
+  <your_wandb_run_name> \
+  <your_output_dir_for_reward_model> \
+  <your_output_dir_for_sft10k> \
+  <kl_coef>
+```
+
 ### OpenAI models
 
 To run the OpenAI reference models with our prompts and decoding hyperparameters, run
 
 ```bash
 python examples/oai_baselines.py \
   --model_name <oai_model_name> \
@@ -328,30 +341,31 @@
 
 You can then use the generated samples at `<save_path>` directly with our automated evaluation.
 
 ## Downloading pre-tuned AlpacaFarm models
 
 We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of
 our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on
-human preference data and release both versions. The current list of models (
-available [here](https://huggingface.co/tatsu-lab)) includes:
+human preference data and release both versions. The current list of models
+(available [here](https://huggingface.co/tatsu-lab)) includes:
 
 - `sft10k`, the supervised learning base model that we collect preference data with.
 - `reward-model-sim`, the reward model trained on AlpacaFarm preference data.
 - `reward-model-human`, the reward model trained on human preference data.
 - `ppo-sim`, the best PPO checkpoint trained in simulation.
 - `ppo-human`, the best PPO checkpoint trained on human data.
 - `expiter-sim`, the best expert iteration checkpoint trained in simulation.
 - `expiter-human`, the best expert iteration checkpoint trained on human data.
 - `feedme-sim`, the FeedME method trained on simulated preferences.
 - `feedme-human`, the FeedME method trained on human preferences.
 - `reward-condition-sim`, the reward conditioning method trained on simulated preferences.
 
-To download these checkpoints, first make sure to have a LLaMA-7B
-checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
+To download and recover these checkpoints, first make sure to have a LLaMA-7B
+checkpoint [converted into the Hugging Face format](https://huggingface.co/docs/transformers/main/model_doc/llama)
+**with transformers>=4.29.2**.
 Then, run the following to download all AlpacaFarm models:
 
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name all
 ```
@@ -364,19 +378,14 @@
   --alpaca-farm-model-name <one_of_the_model_names_from_above> \
   --models-save-dir <dir_to_save_all_models>
 ```
 
 To download either of the reward models individually, you'll need to have `sft10k` downloaded first
 to `<dir_to_save_all_models>`.
 
-## Coming soon
-
-- [ ] Quark implementation
-- [ ] Direct Preference Optimization
-
 ## Citation
 
 Please consider citing our work if you use the data or code in this repo.
 
 ```
 @misc{dubois2023alpacafarm,
       title={AlpacaFarm: A Simulation Framework for Methods that Learn from Human Feedback},
```

### Comparing `alpaca_farm-0.1.3/README.md` & `alpaca_farm-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
 ### RLHF with PPO
 
 To replicate our RLHF PPO model trained with simulated reward model in the paper, run
 
 ```bash
 bash examples/scripts/rlhf_ppo.sh \
-  <your_output_dir> \
+  <your_output_dir_for_ppo> \
   <your_wandb_run_name> \
   <your_output_dir_for_reward_model> \
   <your_output_dir_for_sft10k> \
   <kl_coef>
 ```
 
 `<your_output_dir_for_reward_model>` should point to either simulated reward model or human reward model trained
@@ -295,14 +295,27 @@
 bash examples/scripts/expiter.sh \
   <your_output_dir_for_expiter> \
   <your_wandb_run_name> \
   <your_output_dir_for_sft10k> \
   <your_output_dir_for_expiter_data>
 ```
 
+### Quark
+
+To replicate our Quark results for the AlpacaFarm evaluation suite, run
+
+```bash
+bash examples/scripts/rlhf_quark.sh \
+  <your_output_dir_for_quark> \
+  <your_wandb_run_name> \
+  <your_output_dir_for_reward_model> \
+  <your_output_dir_for_sft10k> \
+  <kl_coef>
+```
+
 ### OpenAI models
 
 To run the OpenAI reference models with our prompts and decoding hyperparameters, run
 
 ```bash
 python examples/oai_baselines.py \
   --model_name <oai_model_name> \
@@ -311,30 +324,31 @@
 
 You can then use the generated samples at `<save_path>` directly with our automated evaluation.
 
 ## Downloading pre-tuned AlpacaFarm models
 
 We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of
 our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on
-human preference data and release both versions. The current list of models (
-available [here](https://huggingface.co/tatsu-lab)) includes:
+human preference data and release both versions. The current list of models
+(available [here](https://huggingface.co/tatsu-lab)) includes:
 
 - `sft10k`, the supervised learning base model that we collect preference data with.
 - `reward-model-sim`, the reward model trained on AlpacaFarm preference data.
 - `reward-model-human`, the reward model trained on human preference data.
 - `ppo-sim`, the best PPO checkpoint trained in simulation.
 - `ppo-human`, the best PPO checkpoint trained on human data.
 - `expiter-sim`, the best expert iteration checkpoint trained in simulation.
 - `expiter-human`, the best expert iteration checkpoint trained on human data.
 - `feedme-sim`, the FeedME method trained on simulated preferences.
 - `feedme-human`, the FeedME method trained on human preferences.
 - `reward-condition-sim`, the reward conditioning method trained on simulated preferences.
 
-To download these checkpoints, first make sure to have a LLaMA-7B
-checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
+To download and recover these checkpoints, first make sure to have a LLaMA-7B
+checkpoint [converted into the Hugging Face format](https://huggingface.co/docs/transformers/main/model_doc/llama)
+**with transformers>=4.29.2**.
 Then, run the following to download all AlpacaFarm models:
 
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name all
 ```
@@ -347,19 +361,14 @@
   --alpaca-farm-model-name <one_of_the_model_names_from_above> \
   --models-save-dir <dir_to_save_all_models>
 ```
 
 To download either of the reward models individually, you'll need to have `sft10k` downloaded first
 to `<dir_to_save_all_models>`.
 
-## Coming soon
-
-- [ ] Quark implementation
-- [ ] Direct Preference Optimization
-
 ## Citation
 
 Please consider citing our work if you use the data or code in this repo.
 
 ```
 @misc{dubois2023alpacafarm,
       title={AlpacaFarm: A Simulation Framework for Methods that Learn from Human Feedback},
```

### Comparing `alpaca_farm-0.1.3/setup.py` & `alpaca_farm-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/__init__.py` & `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-__version__ = "0.1.3"
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/accelerate_patch.py` & `alpaca_farm-0.1.4/src/alpaca_farm/accelerate_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/__init__.py` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .eval import *
 from .pairwise_annotators import *
-from .eval import *
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/analysis.py` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/analysis.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/decoders.py` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/decoders.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/eval.py` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import datasets
 import pandas as pd
 
 from alpaca_farm import constants
 from alpaca_farm.auto_annotations import PairwiseAutoAnnotator
 from alpaca_farm.auto_annotations.analysis import head2head_to_metrics
+
 from . import utils as ann_utils
 
 __all__ = ["alpaca_leaderboard"]
 
 PRECOMPUTED_LEADERBOARD = {
     "annotators/annotator_pool_v0/configs.yaml": {
         # Internal codename: rlhf_llama_7b_regen_v7_3ep_v12_ckpt_20
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/pairwise_annotators.py` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/pairwise_annotators.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import os
 import re
 from pathlib import Path
 from typing import Any, Callable, Optional, Sequence, Union
-import os
 
 import datasets
 import numpy as np
 import pandas as pd
 import yaml
 
-from . import decoders, utils as ann_utils
+from . import decoders
+from . import utils as ann_utils
 
 CURRENT_DIR = Path(__file__).parent
 logging.getLogger().setLevel(logging.INFO)
 
 __all__ = ["PairwiseAutoAnnotator"]
 
 
@@ -88,34 +89,28 @@
 
     decoding_kwargs :
         Additional arguments to pass to `fn_decoder`.
     """
 
     def __init__(
         self,
-        annotators_config: Union[
-            ann_utils.AnyPath, list[dict[str, Any]]
-        ] = "annotators/annotator_pool_v0/configs.yaml",
+        annotators_config: Union[ann_utils.AnyPath, list[dict[str, Any]]] = "annotators/annotator_pool_v0/configs.yaml",
         seed: Optional[int] = None,
         is_avoid_reannotations: bool = True,
         saving_path: Optional[ann_utils.AnyPath] = "auto",
         input_keys: Sequence[str] = ("instruction", "input"),
         output_keys: Sequence[str] = ("output_1", "output_2"),
         p_label_flip: Optional[float] = None,
         **decoding_kwargs,
     ):
         if saving_path == "auto":
             if isinstance(annotators_config, (str, Path, os.PathLike)):
-                saving_path = (
-                    CURRENT_DIR / Path(annotators_config).parent / "annotations.json"
-                )
+                saving_path = CURRENT_DIR / Path(annotators_config).parent / "annotations.json"
             else:
-                logging.warning(
-                    "saving_path cannot be 'auto' if annotators_config is not a path. Setting to None."
-                )
+                logging.warning("saving_path cannot be 'auto' if annotators_config is not a path. Setting to None.")
                 saving_path = None
 
         self.seed = seed
         self.is_avoid_reannotations = is_avoid_reannotations
         self.input_keys = list(input_keys)
         self.output_keys = list(output_keys)
         self.input_output_keys = self.input_keys + self.output_keys
@@ -165,19 +160,15 @@
         decoding_kwargs :
             Additional arguments to pass to the decoder.
         """
 
         all_outputs = ann_utils.convert_to_dataframe(all_outputs)
 
         if is_multisample_list:
-            all_outputs = (
-                all_outputs.explode("output")
-                .reset_index()
-                .rename(columns={"index": "sample_id"})
-            )
+            all_outputs = all_outputs.explode("output").reset_index().rename(columns={"index": "sample_id"})
             all_outputs["sample_id"] = all_outputs.groupby("sample_id").cumcount()
 
         if keys_to_sample_output_2 is None:
             keys_to_sample_output_2 = self.input_keys
         keys_to_sample_output_2 = list(keys_to_sample_output_2)
 
         n_pre_drop = len(all_outputs)
@@ -193,27 +184,23 @@
         if len(df_to_annotate) != n_pre_drop:
             logging.warning(
                 f"""Filtered rows because of duplicate outputs for the same keys_to_sample_output_2=
                 {keys_to_sample_output_2}. {n_pre_drop} -> {len(df_to_annotate)}"""
             )
 
         # sample an output 2 for each output 1 that are different
-        df_to_annotate["output_2"] = df_to_annotate.groupby(
-            list(keys_to_sample_output_2)
-        )["output_1"].transform(
+        df_to_annotate["output_2"] = df_to_annotate.groupby(list(keys_to_sample_output_2))["output_1"].transform(
             lambda x: ann_utils.random_derangement(x.values, seed=self.seed)
         )
 
         if is_unique_instructions:
             n_pre_dedup = len(df_to_annotate)
             df_to_annotate = df_to_annotate.drop_duplicates(subset=self.input_keys)
             if len(df_to_annotate) != n_pre_dedup:
-                logging.info(
-                    f"Filtered unique instruction/input pairs: {n_pre_dedup} -> {len(df_to_annotate)}"
-                )
+                logging.info(f"Filtered unique instruction/input pairs: {n_pre_dedup} -> {len(df_to_annotate)}")
 
         if p_label_flip is not None:
             old_p_label_flip = self.p_label_flip
             self.set_noise(p_label_flip)
 
         try:
             annotated = self.annotate_pairs(df_to_annotate, **decoding_kwargs)
@@ -341,17 +328,15 @@
 
     def _preprocess(self, to_annotate: ann_utils.AnyData) -> pd.DataFrame:
         """Preprocess the examples to annotate. In particular takes care of filtering unnecessary examples."""
 
         df_to_annotate = ann_utils.convert_to_dataframe(to_annotate).copy()
 
         if "preference" in df_to_annotate.columns:
-            logging.warning(
-                """Preference column is already in the dataframe. We will overwrite it."""
-            )
+            logging.warning("""Preference column is already in the dataframe. We will overwrite it.""")
         df_to_annotate["preference"] = np.nan
 
         # remove duplicates because you only need to annotate one of them
         df_to_annotate = df_to_annotate.drop_duplicates(subset=self.input_output_keys)
 
         # set the annotater for each example
         df_to_annotate["annotator"] = df_to_annotate.apply(
@@ -361,32 +346,25 @@
                 choices=list(self.annotators.keys()),
             ),
             axis=1,
         )
 
         if self.is_avoid_reannotations:
             # merge the old annotations
-            df_to_annotate = self._merge_annotations(
-                df_to_annotate, self.df_annotations
-            )
+            df_to_annotate = self._merge_annotations(df_to_annotate, self.df_annotations)
 
         # adds random noise => avoids annotating examples that will be noised out.
         if self.p_label_flip:
-            logging.info(
-                f"Adding random noise to the labels p_label_flip={self.p_label_flip}."
-            )
+            logging.info(f"Adding random noise to the labels p_label_flip={self.p_label_flip}.")
             # if you have 25% change of flipping the label, you have 50% chance of selecting random label
             p_noise = self.p_label_flip * 2
             noisy_preference = df_to_annotate.apply(
                 # we add "noisy_label" at the beginning to use ~independent seeds between tasks
                 lambda x: ann_utils.random_seeded_choice(  # seed on inputs for reproducibility
-                    seed="noisy_preference"
-                    + x["instruction"]
-                    + x["input"]
-                    + str(self.seed),
+                    seed="noisy_preference" + x["instruction"] + x["input"] + str(self.seed),
                     choices=[np.nan, 1, 2],
                     p=[1 - p_noise, self.p_label_flip, self.p_label_flip],
                 ),
                 axis=1,
             )
             df_to_annotate["is_noisy_label"] = ~noisy_preference.isna()
             # keeps previously annotated examples when you did not add noise
@@ -413,57 +391,45 @@
                     logging.exception(exc)
 
         return {
             name: SinglePairwiseAutoAnnotator(**annotator_config)
             for name, annotator_config in annotators_config.items()
         }
 
-    def _annotate(
-        self, df_to_annotate: pd.DataFrame, **decoding_kwargs
-    ) -> pd.DataFrame:
+    def _annotate(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
         """Annotate the examples."""
         curr_decoding_kwargs = self.decoding_kwargs
         curr_decoding_kwargs.update(decoding_kwargs)
 
         df_annotated = df_to_annotate
         for annotator in self.annotators.keys():
             # only annotate examples that have not been annotated yet
-            curr_idcs = (df_annotated["annotator"] == annotator) & df_annotated[
-                "preference"
-            ].isna()
+            curr_idcs = (df_annotated["annotator"] == annotator) & df_annotated["preference"].isna()
 
             logging.info(f"Annotating {curr_idcs.sum()} examples with {annotator}")
 
             # actual annotation
-            curr_annotated = self.annotators[annotator](
-                df_annotated[curr_idcs], **curr_decoding_kwargs
-            )
+            curr_annotated = self.annotators[annotator](df_annotated[curr_idcs], **curr_decoding_kwargs)
 
             df_annotated = self._merge_annotations(df_annotated, curr_annotated)
 
         return df_annotated
 
-    def _postprocess_and_store_(
-        self, df_annotated: pd.DataFrame
-    ) -> list[dict[str, Any]]:
+    def _postprocess_and_store_(self, df_annotated: pd.DataFrame) -> list[dict[str, Any]]:
         """Convert the dataframe into a list of dictionaries to be returned, and store current anntations."""
 
         # select available annotations
         df_annotated = df_annotated[~df_annotated["preference"].isna()].copy()
 
         # try converting to int now that no nan
-        df_annotated["preference"] = pd.to_numeric(
-            df_annotated["preference"], downcast="integer", errors="ignore"
-        )
+        df_annotated["preference"] = pd.to_numeric(df_annotated["preference"], downcast="integer", errors="ignore")
 
         if "is_noisy_label" in df_annotated.columns:
             # dont' store noisy labels
-            df_annotated_to_store = df_annotated.query("is_noisy_label == False").drop(
-                columns=["is_noisy_label"]
-            )
+            df_annotated_to_store = df_annotated.query("is_noisy_label == False").drop(columns=["is_noisy_label"])
             df_annotated = df_annotated.drop(columns=["is_noisy_label"])
         else:
             df_annotated_to_store = df_annotated
 
         if self.df_annotations is None:
             self.df_annotations = df_annotated_to_store
         else:
@@ -489,33 +455,27 @@
         path = path or self.saving_path
         if path is not None:
             path = Path(path)
             if path.exists():
                 logging.info(f"Loading all annotations from {path}.")
                 self.df_annotations = pd.read_json(path)
 
-    def _merge_annotations(
-        self, df_to_annotate: pd.DataFrame, df_partially_annotated: pd.DataFrame
-    ) -> pd.DataFrame:
+    def _merge_annotations(self, df_to_annotate: pd.DataFrame, df_partially_annotated: pd.DataFrame) -> pd.DataFrame:
         """Merge (partial) annotations with the original df to keep the same order and avoid duplicates annotations."""
         if df_partially_annotated is None or df_partially_annotated.empty:
             return df_to_annotate
 
         df_to_annotate = df_to_annotate.merge(
             df_partially_annotated[self.all_keys + ["preference"]],
             on=self.all_keys,
             how="left",
             suffixes=("_old", "_new"),
         )
-        df_to_annotate["preference"] = df_to_annotate["preference_old"].fillna(
-            df_to_annotate["preference_new"]
-        )
-        df_to_annotate = df_to_annotate.drop(
-            columns=["preference_old", "preference_new"]
-        )
+        df_to_annotate["preference"] = df_to_annotate["preference_old"].fillna(df_to_annotate["preference_new"])
+        df_to_annotate = df_to_annotate.drop(columns=["preference_old", "preference_new"])
         return df_to_annotate
 
 
 class SinglePairwiseAutoAnnotator:
     """A helper class for a single auto annotators.
 
     Parameters
@@ -555,16 +515,15 @@
         decoder_kwargs: Optional[dict[str, Any]] = None,
         is_randomize_output_order: bool = True,
         is_shuffle: bool = True,
         seed: Optional[int] = None,
         batch_size: int = 1,
     ):
         self.prompt_templates = {
-            k: ann_utils.read_or_return(CURRENT_DIR / prompt)
-            for k, prompt in prompt_templates.items()
+            k: ann_utils.read_or_return(CURRENT_DIR / prompt) for k, prompt in prompt_templates.items()
         }
         self.outputs_to_match = {k: re.compile(v) for k, v in outputs_to_match.items()}
         self.is_randomize_output_order = is_randomize_output_order
         self.fn_decoder = getattr(decoders, fn_decoder, fn_decoder)
         self.decoder_kwargs = decoder_kwargs or {}
         self.seed = seed
         self.is_shuffle = is_shuffle
@@ -588,17 +547,15 @@
             return df_to_annotate
 
         df_to_annotate = self.preprocess(df_to_annotate)
 
         # prompts and completions here will not be the same length as the dataframe due to batching
         prompts, df_to_annotate = self.make_prompts(df_to_annotate=df_to_annotate)
 
-        completions = self.fn_decoder(
-            prompts=prompts, **self.decoder_kwargs, **decoding_kwargs
-        )
+        completions = self.fn_decoder(prompts=prompts, **self.decoder_kwargs, **decoding_kwargs)
 
         df_to_annotate["preference"] = self.parse_completions(completions=completions)
 
         df_annotated = self.postprocess(df_to_annotate)
 
         return df_annotated
 
@@ -606,34 +563,29 @@
         """Preprocess the examples before annotating. In particular, takes care of all the randomization."""
 
         if self.is_randomize_output_order:
             # randomize order of output_1, output_2 base on inputs
             df_to_annotate["is_switched_outputs"] = df_to_annotate.apply(
                 # we add "is_switched_outputs" at the beginning to not use the same seed for all tasks
                 lambda x: ann_utils.random_seeded_choice(
-                    seed="is_switched_outputs"
-                    + x["instruction"]
-                    + x["input"]
-                    + str(self.seed),
+                    seed="is_switched_outputs" + x["instruction"] + x["input"] + str(self.seed),
                     choices=[False, True],
                 ),
                 axis=1,
             )
             df_to_annotate = ann_utils.shuffle_pairwise_preferences(
                 df_to_annotate, df_to_annotate["is_switched_outputs"]
             )
 
         if self.is_shuffle:
             df_to_annotate = df_to_annotate.sample(frac=1, random_state=self.seed)
 
         return df_to_annotate
 
-    def make_prompts(
-        self, df_to_annotate: pd.DataFrame
-    ) -> tuple[list[str], pd.DataFrame]:
+    def make_prompts(self, df_to_annotate: pd.DataFrame) -> tuple[list[str], pd.DataFrame]:
         """Make all the prompts for the given examples.
 
         Parameters
         ----------
         df_to_annotate : pd.DataFrame
             Examples to annotate
 
@@ -641,17 +593,15 @@
         -------
         prompts : list[str]
             Formatted prompts for the given examples.
 
         df_to_annotate : pd.DataFrame
             Examples to annotate in the same order as prompts.
         """
-        arr_is_inputs = (df_to_annotate["input"] != "") & (
-            df_to_annotate["input"].notnull()
-        )
+        arr_is_inputs = (df_to_annotate["input"] != "") & (df_to_annotate["input"].notnull())
         df_with_inputs = df_to_annotate[arr_is_inputs]
         df_without_inputs = df_to_annotate[~arr_is_inputs]
 
         prompts, df = ann_utils.make_prompts(
             df_without_inputs,
             self.prompt_templates["without_inputs"],
             batch_size=self.batch_size,
@@ -668,45 +618,39 @@
         return prompts, df
 
     def parse_completions(self, completions: list[str]) -> list[int]:
         """Converts the completions into annotations."""
         all_preferences = []
         for completion in completions:
             # use a regex to match all outputs on a line. Assumes that there is at most one output to match per line
-            batch_preferences = ann_utils.parse_batched_completion(
-                completion, self.outputs_to_match
-            )
+            batch_preferences = ann_utils.parse_batched_completion(completion, self.outputs_to_match)
             if len(batch_preferences) != self.batch_size:
                 logging.warning(
                     f"""Found {len(batch_preferences)} preferences in:\n{completion} but expected {self.batch_size}.
                     We are setting all preferences to np.nan."""
                 )
                 batch_preferences = [np.nan] * self.batch_size
             all_preferences += batch_preferences
         return all_preferences
 
     def postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         """Postprocess the annotated examples."""
 
         # remove padding examples when using batch_size > 1
-        df_annotated = df_annotated.query("is_padding == False").drop(
-            columns=["is_padding"]
-        )
+        df_annotated = df_annotated.query("is_padding == False").drop(columns=["is_padding"])
 
         arr_is_na = df_annotated["preference"].isna()
         if arr_is_na.any():
             logging.warning(
                 f"{arr_is_na.sum().item()} samples had no auto annotation. We are filtering them for now. "
                 f"If you are using chain of thought it might be that max_tokens limit is too low. "
             )
             df_annotated = df_annotated[~arr_is_na]
 
         assert set(df_annotated["preference"].unique().tolist()) <= {1, 2}
 
         if self.is_randomize_output_order:
             # unshuffles output 1 and output 2. For binary preference, unshuffling is equivalent to reshuffling
-            df_annotated = ann_utils.shuffle_pairwise_preferences(
-                df_annotated, df_annotated["is_switched_outputs"]
-            )
+            df_annotated = ann_utils.shuffle_pairwise_preferences(df_annotated, df_annotated["is_switched_outputs"])
             df_annotated = df_annotated.drop(columns=["is_switched_outputs"])
 
         return df_annotated
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/utils.py` & `alpaca_farm-0.1.4/src/alpaca_farm/auto_annotations/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import itertools
 import logging
-import random
 import os
 import pathlib
+import random
 import re
 from collections import Counter
 from pathlib import Path
 from typing import Any, Sequence, Union
 
 import datasets
 import numpy as np
@@ -269,18 +269,19 @@
     preferences[binary_preference_key] = (preferences[ordinal_preference_key].round().astype(int) - 1) // 2 + 1
 
     if not is_df:
         preferences = preferences.to_dict(orient="records")
 
     return preferences
 
-def convert_to_dataframe(data : AnyData) -> pd.DataFrame:
+
+def convert_to_dataframe(data: AnyData) -> pd.DataFrame:
     """Convert input that AlpacaFarm accepts into a dataframe."""
     if isinstance(data, pd.DataFrame):
         return data
     elif isinstance(data, datasets.Dataset):
         return data.data.to_pandas()
     elif isinstance(data, list):
         return pd.DataFrame.from_records(data)
     else:
         # try
-        return pd.DataFrame(data)
+        return pd.DataFrame(data)
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/common.py` & `alpaca_farm-0.1.4/src/alpaca_farm/common.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/constants.py` & `alpaca_farm-0.1.4/src/alpaca_farm/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/data_postprocessor.py` & `alpaca_farm-0.1.4/src/alpaca_farm/data_postprocessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,7 +36,15 @@
                 special_tokens.extend(operation.special_tokens)
         self.special_tokens = special_tokens
 
     def __call__(self, df: Union[pd.DataFrame, dict]) -> Union[pd.DataFrame, dict]:
         for operation in self.operations:
             df = operation(df)
         return df
+
+
+@dataclass
+class RewardConditioningPromptPostprocessor(object):
+    injected_token = "<reward_0>"
+
+    def __call__(self, prompt: str, **kwargs):
+        return f"{self.injected_token}{prompt}"
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/data_preprocessor.py` & `alpaca_farm-0.1.4/src/alpaca_farm/data_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -411,37 +411,37 @@
             attention_mask=attention_mask,
             index_0=index_0,
             index_1=index_1,
             choice=choice,
         )
 
 
-class QueryResponseDataset(Dataset):
+class QueryDataset(Dataset):
     """Dataset that emits tokenized left-padded queries."""
 
     def __init__(
         self,
         df: pd.DataFrame,
         prompt_dict: dict,
         tokenizer: transformers.PreTrainedTokenizer,
         query_len: int,
         df_postprocessor: Optional[Callable] = None,
+        prompt_postprocessor: Optional[Callable] = None,
     ):
-        super(QueryResponseDataset, self).__init__()
+        super(QueryDataset, self).__init__()
 
         if df_postprocessor is not None:
             df = df_postprocessor(df)
         list_dict_data = df.to_dict(orient="records")
 
-        # prompts are strings; queries are tensors.
         prompts = [format_prompt(example=dict_data, prompt_dict=prompt_dict) for dict_data in list_dict_data]
-        queries = [
-            tokenizer(prompt, return_tensors="pt", truncation=False).input_ids.squeeze(dim=0) for prompt in prompts
-        ]
+        if prompt_postprocessor is not None:
+            prompts = [prompt_postprocessor(prompt) for prompt in prompts]
 
+        queries = [tokenizer(prompt, return_tensors="pt", truncation=False).input_ids[0] for prompt in prompts]
         filtered_queries = [query for query in queries if len(query) <= query_len]
         logger.warning(
             f"Filtered out {len(queries) - len(filtered_queries)} instances out of {len(queries)} that "
             f"exceed length limit. These examples are not used for training, but will still be used in evaluation. "
         )
 
         queries = torch.stack(
@@ -455,18 +455,74 @@
         self.query_attn_masks = queries.ne(tokenizer.pad_token_id).long()
 
         # Auxiliary data.
         self.prompts = prompts
         self.list_dict_data = list_dict_data
 
     def __getitem__(self, i):
-        return_dict = dict(queries=self.queries[i], query_attn_masks=self.query_attn_masks[i])
-        return return_dict
+        return dict(queries=self.queries[i], query_attn_masks=self.query_attn_masks[i])
+
+    def __len__(self):
+        return len(self.queries)
+
+
+class QueryResponseDataset(Dataset):
+    def __init__(
+        self,
+        tokenizer: transformers.PreTrainedTokenizer,
+        queries: Sequence[str],
+        responses: Sequence[str],
+        query_len: int,
+        response_len: int,
+    ):
+        super(QueryResponseDataset, self).__init__()
+
+        def tokenize_without_truncation(strings):
+            return [tokenizer(string, return_tensors="pt", truncation=False).input_ids[0] for string in strings]
+
+        sequences = [query + response for query, response in utils.zip_(queries, responses)]
+
+        queries = tokenize_without_truncation(queries)
+        sequences = tokenize_without_truncation(sequences)
+        responses = [sequence[len(query) :] for sequence, query in utils.zip_(sequences, queries)]
+
+        filtered_pairs = [
+            (query, response)
+            for query, response in utils.zip_(queries, responses)
+            if len(query) <= query_len and len(response) <= response_len
+        ]
+        filtered_queries = [query for query, _ in filtered_pairs]
+        filtered_responses = [response for _, response in filtered_pairs]
+
+        logger.warning(
+            f"Filtered out {len(queries) - len(filtered_queries)} instances out of {len(queries)} that "
+            f"exceed length limit... "
+            f"These examples are not used for training. "
+            f"However they won't be ignored if this is eval set that is used in `RLTrainer.evaluate`."
+        )
+
+        def left_pad_and_stack(list_of_tensors: Sequence[torch.Tensor], target_len: int):
+            return torch.stack(
+                [
+                    torch_ops.left_pad(tensor, target_size=(target_len,), value=tokenizer.pad_token_id)
+                    for tensor in list_of_tensors
+                ]
+            )
+
+        queries = left_pad_and_stack(filtered_queries, query_len)
+        responses = left_pad_and_stack(filtered_responses, response_len)
+
+        self.queries = queries
+        self.responses = responses
+        self.query_attn_masks = queries.ne(tokenizer.pad_token_id).long()
+
+    def __getitem__(self, i):
+        return dict(queries=self.queries[i], responses=self.responses[i], query_attn_masks=self.query_attn_masks[i])
 
     def __len__(self):
         return len(self.queries)
 
 
 @dataclasses.dataclass
-class DataCollatorForQueryResponseDataset(object):
+class DataCollatorForStackableDataset(object):
     def __call__(self, instances: Sequence[Dict]) -> Dict[str, Tensor]:
         return {key: torch.stack([instance[key] for instance in instances]) for key in instances[0].keys()}
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/data_utils.py` & `alpaca_farm-0.1.4/src/alpaca_farm/data_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datasets
 import pandas as pd
 import transformers
 
-from . import utils, logging
+from . import logging, utils
+from .data_postprocessor import RewardConditioningPromptPostprocessor
 from .data_preprocessor import (
     BinaryRewardModelingDataset,
     DataCollatorForBinaryRewardModelingDataset,
-    DataCollatorForQueryResponseDataset,
     DataCollatorForSFTDataset,
-    QueryResponseDataset,
+    DataCollatorForStackableDataset,
+    QueryDataset,
     SFTDataset,
     split_train_into_train_and_eval,
 )
 
 logger = logging.get_logger(__name__)
 
 
@@ -99,22 +100,29 @@
 ):
     prompt_dict = utils.jload(data_args.prompt_dict_path)
 
     alpaca_instructions = datasets.load_dataset(data_args.dataset_path, data_args.dataset_name)
     train_df = pd.concat([pd.DataFrame(alpaca_instructions[split]) for split in data_args.train_splits])
     eval_df = pd.concat([pd.DataFrame(alpaca_instructions[split]) for split in data_args.eval_splits])
 
-    train_dataset = QueryResponseDataset(
+    if getattr(training_args, "num_reward_tokens", 0) > 0 and not getattr(
+        training_args, "train_on_best_quantile", True
+    ):
+        prompt_postprocessor = RewardConditioningPromptPostprocessor()
+    else:
+        prompt_postprocessor = None
+
+    train_dataset = QueryDataset(
         df=train_df,
         prompt_dict=prompt_dict,
         tokenizer=tokenizer,
         query_len=training_args.query_len,
+        prompt_postprocessor=prompt_postprocessor,
     )
-    eval_dataset = QueryResponseDataset(
+    eval_dataset = QueryDataset(
         df=eval_df,
         prompt_dict=prompt_dict,
         tokenizer=tokenizer,
         query_len=training_args.query_len,
+        prompt_postprocessor=prompt_postprocessor,
     )
-    return dict(
-        train_dataset=train_dataset, eval_dataset=eval_dataset, data_collator=DataCollatorForQueryResponseDataset()
-    )
+    return dict(train_dataset=train_dataset, eval_dataset=eval_dataset, data_collator=DataCollatorForStackableDataset())
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/distributed_utils.py` & `alpaca_farm-0.1.4/src/alpaca_farm/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/__init__.py` & `alpaca_farm-0.1.4/src/alpaca_farm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/apex_patch.py` & `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/apex_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_llama.py` & `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_opt.py` & `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/tensor_ops.py` & `alpaca_farm-0.1.4/src/alpaca_farm/flash_models/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/inference/__init__.py` & `alpaca_farm-0.1.4/src/alpaca_farm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/inference/decode.py` & `alpaca_farm-0.1.4/src/alpaca_farm/inference/decode.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/inference/score.py` & `alpaca_farm-0.1.4/src/alpaca_farm/inference/score.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/logging.py` & `alpaca_farm-0.1.4/src/alpaca_farm/logging.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/models/__init__.py` & `alpaca_farm-0.1.4/src/alpaca_farm/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/models/reward_model.py` & `alpaca_farm-0.1.4/src/alpaca_farm/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/models/rl_models.py` & `alpaca_farm-0.1.4/src/alpaca_farm/models/rl_models.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/openai_utils.py` & `alpaca_farm-0.1.4/src/alpaca_farm/openai_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     return return_data
 
 
 def _openai_completion_helper(
     prompt_batch: Sequence[StrOrOpenAIObject],
     is_chat: bool,
     sleep_time: int,
-    openai_organization_ids : Optional[Sequence[str]]= None,
+    openai_organization_ids: Optional[Sequence[str]] = None,
     openai_api_key: Optional[str] = None,
     **shared_kwargs,
 ):
     if openai_api_key is not None:
         openai.api_key = openai_api_key
 
     # randomly select orgs
@@ -128,15 +128,17 @@
             logging.warning(f"OpenAIError: {e}.")
             if "Please reduce your prompt" in str(e):
                 shared_kwargs["max_tokens"] = int(shared_kwargs["max_tokens"] * 0.8)
                 logging.warning(f"Reducing target length to {shared_kwargs['max_tokens']}, Retrying...")
             else:
                 logging.warning("Hit request rate limit; retrying...")
                 if openai_organization_ids is not None and len(openai_organization_ids) > 1:
-                    openai.organization = random.choice([o for o in openai_organization_ids if o != openai.organization])
+                    openai.organization = random.choice(
+                        [o for o in openai_organization_ids if o != openai.organization]
+                    )
                     logging.warning(f"Switching to organization: {openai.organization} for OAI API key.")
                 time.sleep(sleep_time)  # Annoying rate limit on requests.
     return choices
 
 
 def _openai_completion(
     prompts: Union[str, Sequence[str], Sequence[dict[str, str]], dict[str, str]],
@@ -205,18 +207,15 @@
     shared_kwargs = dict(
         model=model_name,
         **decoding_args.__dict__,
     )
     shared_kwargs.update(decoding_kwargs)  # override default arguments if specified
     with multiprocessing.Pool(num_procs) as p:
         partial_completion_helper = functools.partial(
-            _openai_completion_helper,
-            sleep_time=sleep_time,
-            is_chat=is_chat,
-            **shared_kwargs
+            _openai_completion_helper, sleep_time=sleep_time, is_chat=is_chat, **shared_kwargs
         )
         completions = list(
             tqdm.tqdm(
                 p.imap(partial_completion_helper, prompt_batches),
                 desc="prompt_batches",
                 total=len(prompt_batches),
             )
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/reward_modeling_trainer.py` & `alpaca_farm-0.1.4/src/alpaca_farm/reward_modeling_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/rl/__init__.py` & `alpaca_farm-0.1.4/src/alpaca_farm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = "0.1.4"
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/rl/kl_controller.py` & `alpaca_farm-0.1.4/src/alpaca_farm/rl/kl_controller.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_trainer.py` & `alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Callable, Dict, Optional, Tuple
 
 import accelerate
 import pandas as pd
 import torch
 import tqdm
 import transformers
+from torch import nn
 from torch.distributed.fsdp.fully_sharded_data_parallel import FullStateDictConfig
 from torch.distributed.fsdp.fully_sharded_data_parallel import FullyShardedDataParallel as FSDP
 from torch.distributed.fsdp.fully_sharded_data_parallel import StateDictType
 from transformers.modeling_utils import unwrap_model
 
 from .. import accelerate_patch, common, constants, data_preprocessor, logging, torch_ops, utils
 from ..models import reward_model as reward_model_module
@@ -34,20 +35,20 @@
 logger = logging.get_logger(__name__)
 
 
 class PPOTrainer(rl_trainer.RLTrainer):
     def __init__(
         self,
         args,
-        train_dataset: data_preprocessor.QueryResponseDataset,
-        eval_dataset: data_preprocessor.QueryResponseDataset,
+        train_dataset: data_preprocessor.QueryDataset,
+        eval_dataset: data_preprocessor.QueryDataset,
         data_collator: Callable,
         policy: rl_models.ActorCritic,
         ref_policy: rl_models.Policy,
-        reward_model,
+        reward_model: nn.Module,
         tokenizer: transformers.PreTrainedTokenizer,
         accelerator: accelerate_patch.MyAccelerator,
         optimizer: Optional[torch.optim.Optimizer] = None,
         lr_scheduler: Optional[LRScheduler] = None,
     ):
         super(PPOTrainer, self).__init__(
             args=args,
@@ -450,14 +451,14 @@
     ref_policy.requires_grad_(False)
     ref_policy = accelerator.prepare(ref_policy)  # noqa
 
     reward_model = make_reward_model()
     reward_model.requires_grad_(False)
     reward_model = accelerator.prepare(reward_model)
 
-    # TODO: This is a hack to get FSDP running. Remove in the future when we figure things out.
+    # TODO: This is a hack to get FSDP running. Remove in the future when this is fixed.
     if accelerator.distributed_type == accelerate.DistributedType.FSDP:
         inputs = tokenizer("fsdp are you happy now??? :)" * 50, return_tensors="pt")
         inputs = {key: value.to(accelerator.device) for key, value in inputs.items()}
         actor_critic(inputs["input_ids"], inputs["attention_mask"], inputs["input_ids"])
 
     return dict(policy=actor_critic, ref_policy=ref_policy, reward_model=reward_model)
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_utils.py` & `alpaca_farm-0.1.4/src/alpaca_farm/rl/ppo_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/rl/rl_trainer.py` & `alpaca_farm-0.1.4/src/alpaca_farm/rl/rl_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 logger = logging.get_logger(__name__)
 
 
 class RLTrainer(object):
     def __init__(
         self,
         args,
-        train_dataset: data_preprocessor.QueryResponseDataset,
-        eval_dataset: data_preprocessor.QueryResponseDataset,
+        train_dataset: data_preprocessor.QueryDataset,
+        eval_dataset: data_preprocessor.QueryDataset,
         data_collator: Callable,
         policy: nn.Module,
         ref_policy: nn.Module,
         reward_model: nn.Module,
         tokenizer: transformers.PreTrainedTokenizer,
         accelerator: accelerate_patch.MyAccelerator,
         optimizer: Optional[torch.optim.Optimizer] = None,
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/torch_ops.py` & `alpaca_farm-0.1.4/src/alpaca_farm/torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/trainer_utils.py` & `alpaca_farm-0.1.4/src/alpaca_farm/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/types.py` & `alpaca_farm-0.1.4/src/alpaca_farm/types.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import pathlib
 from typing import Any, List, Optional, Sequence, Union
 
+import datasets
 import pandas as pd
 import torch
-import datasets
 from torch import Tensor
 
 AnyPath = Union[str, os.PathLike, pathlib.Path]
 AnyPathOrNone = Optional[AnyPath]
 AnyData = Union[Sequence[dict[str, Any]], pd.DataFrame, datasets.Dataset]
 
 Numeric = Union[int, float]
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm/utils.py` & `alpaca_farm-0.1.4/src/alpaca_farm/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -127,36 +127,35 @@
 
     For new tokens, the embedding value is the average of all old embedding vectors.
     """
     tokenizer.add_special_tokens(special_tokens_dict)
     stable_resize_token_embeddings(model, len(tokenizer))
 
 
-def stable_resize_token_embeddings(
-    model: transformers.PreTrainedModel, target_size: int
-):
+def stable_resize_token_embeddings(model: transformers.PreTrainedModel, target_size: int, jitter_new_embeddings=False):
     num_new_tokens = target_size - model.get_input_embeddings().weight.size(0)
     model.resize_token_embeddings(target_size)
 
-    # New token embedding takes the average of existing ones.
-    # We need this check since `num_new_tokens` can be negative if token embeddings were padded initially.
-    # This can happen when there's multiple-of-64 padding.
     if num_new_tokens > 0:
-        input_embeddings = model.get_input_embeddings().weight.data
-        output_embeddings = model.get_output_embeddings().weight.data
 
-        input_embeddings_avg = input_embeddings[:-num_new_tokens].mean(
-            dim=0, keepdim=True
-        )
-        output_embeddings_avg = output_embeddings[:-num_new_tokens].mean(
-            dim=0, keepdim=True
-        )
-
-        input_embeddings[-num_new_tokens:] = input_embeddings_avg
-        output_embeddings[-num_new_tokens:] = output_embeddings_avg
+        @torch.inference_mode()
+        def stable_init(embedding):
+            embedding_data = embedding.weight.data
+            embedding_avg = embedding_data[:-num_new_tokens].mean(dim=0, keepdim=True)
+            embedding_data[-num_new_tokens:] = embedding_avg
+            if jitter_new_embeddings:
+                embedding_std = embedding_data[:-num_new_tokens].std(dim=0, keepdim=True)
+                # The random tensor must be of the same shape as the new embeddings.
+                embedding_data[-num_new_tokens:] += torch.randn_like(embedding_data[-num_new_tokens:]) * embedding_std
+
+        input_embeddings = model.get_input_embeddings()  # Must grab this again after resize.
+        output_embeddings = model.get_output_embeddings()
+        # It doesn't matter if there's weight sharing or not; with sharing, the second init will overwrite the first.
+        for embeddings in (input_embeddings, output_embeddings):
+            stable_init(embeddings)
 
 
 def convert_str_dtype_to_torch_dtype(str_dtype: Optional[str]):
     if str_dtype in ("single", "float32", "float", "fp32", None):
         return torch.float
     elif str_dtype in ("half", "float16", "fp16"):
         return torch.float16
@@ -191,7 +190,16 @@
 
     def __next__(self):
         try:
             return next(self.iterator)
         except StopIteration:
             self.iterator = iter(self.loader)
             return next(self.iterator)
+
+
+def parallel_sort(*args: Sequence, key=None, reverse=False):
+    """Parallel sort of multiple lists."""
+    if key is None:
+        # Parallel sort based on the order of the first list.
+        key = lambda inputs: inputs[0]  # noqa
+    ret = sorted(zip_(*args), key=key, reverse=reverse)
+    return tuple([ret_i[j] for ret_i in ret] for j in range(len(args)))
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm.egg-info/PKG-INFO` & `alpaca_farm-0.1.4/src/alpaca_farm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-farm
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -249,15 +249,15 @@
 
 ### RLHF with PPO
 
 To replicate our RLHF PPO model trained with simulated reward model in the paper, run
 
 ```bash
 bash examples/scripts/rlhf_ppo.sh \
-  <your_output_dir> \
+  <your_output_dir_for_ppo> \
   <your_wandb_run_name> \
   <your_output_dir_for_reward_model> \
   <your_output_dir_for_sft10k> \
   <kl_coef>
 ```
 
 `<your_output_dir_for_reward_model>` should point to either simulated reward model or human reward model trained
@@ -312,14 +312,27 @@
 bash examples/scripts/expiter.sh \
   <your_output_dir_for_expiter> \
   <your_wandb_run_name> \
   <your_output_dir_for_sft10k> \
   <your_output_dir_for_expiter_data>
 ```
 
+### Quark
+
+To replicate our Quark results for the AlpacaFarm evaluation suite, run
+
+```bash
+bash examples/scripts/rlhf_quark.sh \
+  <your_output_dir_for_quark> \
+  <your_wandb_run_name> \
+  <your_output_dir_for_reward_model> \
+  <your_output_dir_for_sft10k> \
+  <kl_coef>
+```
+
 ### OpenAI models
 
 To run the OpenAI reference models with our prompts and decoding hyperparameters, run
 
 ```bash
 python examples/oai_baselines.py \
   --model_name <oai_model_name> \
@@ -328,30 +341,31 @@
 
 You can then use the generated samples at `<save_path>` directly with our automated evaluation.
 
 ## Downloading pre-tuned AlpacaFarm models
 
 We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of
 our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on
-human preference data and release both versions. The current list of models (
-available [here](https://huggingface.co/tatsu-lab)) includes:
+human preference data and release both versions. The current list of models
+(available [here](https://huggingface.co/tatsu-lab)) includes:
 
 - `sft10k`, the supervised learning base model that we collect preference data with.
 - `reward-model-sim`, the reward model trained on AlpacaFarm preference data.
 - `reward-model-human`, the reward model trained on human preference data.
 - `ppo-sim`, the best PPO checkpoint trained in simulation.
 - `ppo-human`, the best PPO checkpoint trained on human data.
 - `expiter-sim`, the best expert iteration checkpoint trained in simulation.
 - `expiter-human`, the best expert iteration checkpoint trained on human data.
 - `feedme-sim`, the FeedME method trained on simulated preferences.
 - `feedme-human`, the FeedME method trained on human preferences.
 - `reward-condition-sim`, the reward conditioning method trained on simulated preferences.
 
-To download these checkpoints, first make sure to have a LLaMA-7B
-checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
+To download and recover these checkpoints, first make sure to have a LLaMA-7B
+checkpoint [converted into the Hugging Face format](https://huggingface.co/docs/transformers/main/model_doc/llama)
+**with transformers>=4.29.2**.
 Then, run the following to download all AlpacaFarm models:
 
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name all
 ```
@@ -364,19 +378,14 @@
   --alpaca-farm-model-name <one_of_the_model_names_from_above> \
   --models-save-dir <dir_to_save_all_models>
 ```
 
 To download either of the reward models individually, you'll need to have `sft10k` downloaded first
 to `<dir_to_save_all_models>`.
 
-## Coming soon
-
-- [ ] Quark implementation
-- [ ] Direct Preference Optimization
-
 ## Citation
 
 Please consider citing our work if you use the data or code in this repo.
 
 ```
 @misc{dubois2023alpacafarm,
       title={AlpacaFarm: A Simulation Framework for Methods that Learn from Human Feedback},
```

### Comparing `alpaca_farm-0.1.3/src/alpaca_farm.egg-info/SOURCES.txt` & `alpaca_farm-0.1.4/src/alpaca_farm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,11 +68,14 @@
 src/alpaca_farm/models/__init__.py
 src/alpaca_farm/models/reward_model.py
 src/alpaca_farm/models/rl_models.py
 src/alpaca_farm/rl/__init__.py
 src/alpaca_farm/rl/kl_controller.py
 src/alpaca_farm/rl/ppo_trainer.py
 src/alpaca_farm/rl/ppo_utils.py
+src/alpaca_farm/rl/quark_trainer.py
+src/alpaca_farm/rl/quark_utils.py
 src/alpaca_farm/rl/rl_trainer.py
 tests/test_flash_llama.py
 tests/test_flash_opt.py
-tests/test_torch_ops.py
+tests/test_torch_ops.py
+tests/test_utils.py
```

### Comparing `alpaca_farm-0.1.3/tests/test_flash_llama.py` & `alpaca_farm-0.1.4/tests/test_flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/tests/test_flash_opt.py` & `alpaca_farm-0.1.4/tests/test_flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.3/tests/test_torch_ops.py` & `alpaca_farm-0.1.4/tests/test_torch_ops.py`

 * *Files identical despite different names*

