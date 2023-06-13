# Comparing `tmp/xturing-0.1.3.tar.gz` & `tmp/xturing-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.1.3.tar", last modified: Thu May 11 14:52:21 2023, max compression
+gzip compressed data, was "xturing-0.1.4.tar", last modified: Tue Jun 13 14:43:38 2023, max compression
```

## Comparing `xturing-0.1.3.tar` & `xturing-0.1.4.tar`

### file list

```diff
@@ -1,114 +1,118 @@
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.955321 xturing-0.1.3/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-03-20 17:06:03.000000 xturing-0.1.3/LICENSE
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-03-29 09:39:04.000000 xturing-0.1.3/MANIFEST.in
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21623 2023-05-11 14:52:21.955321 xturing-0.1.3/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7161 2023-05-11 14:51:34.000000 xturing-0.1.3/README.md
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-05-11 14:51:34.000000 xturing-0.1.3/pyproject.toml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-05-11 14:52:21.955321 xturing-0.1.3/setup.cfg
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.915321 xturing-0.1.3/src/
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.923321 xturing-0.1.3/src/xturing/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/__about__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/__init__.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.927321 xturing-0.1.3/src/xturing/cli/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/cli/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/cli/api.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/cli/chat.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/cli/ui.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.927321 xturing-0.1.3/src/xturing/config/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/config/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/config/config_data_classes.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2701 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/config/finetuning_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2517 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/config/generation_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1862 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/config/read_config.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.931321 xturing-0.1.3/src/xturing/datasets/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/datasets/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/datasets/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8187 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/datasets/instruction_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/datasets/text2image_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/datasets/text_dataset.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.935321 xturing-0.1.3/src/xturing/engines/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3182 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/engines/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/bloom_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6866 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/engines/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/cerebras_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/distilgpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/galactica_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/gpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/gptj_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.935321 xturing-0.1.3/src/xturing/engines/gptj_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/engines/gptj_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/gptj_utils/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6306 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/engines/llama_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.935321 xturing-0.1.3/src/xturing/engines/llama_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/engines/llama_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    44486 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/engines/llama_utils/llama.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.939321 xturing-0.1.3/src/xturing/engines/lora_engine/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/lora.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/save_and_load.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/test.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/opt_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.939321 xturing-0.1.3/src/xturing/engines/quant_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/quant_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6803 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/quant_utils/custom_autotune.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/quant_utils/quant.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.943321 xturing-0.1.3/src/xturing/model_apis/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/ai21.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/cohere.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/openai.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.947321 xturing-0.1.3/src/xturing/models/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2566 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/models/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/models/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/bloom.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7471 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/models/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/cerebras.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/distilgpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/galactica.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/gpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2259 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/models/llama.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/opt.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/models/stable_diffusion.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.947321 xturing-0.1.3/src/xturing/preprocessors/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/preprocessors/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/preprocessors/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/preprocessors/instruction_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/preprocessors/text_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/registry.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/self_instruct/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/bootstrap_instructions.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/generate_instances.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/identify_if_classification.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/self_instruct/templates/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/templates/clf_task_template.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/trainers/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/trainers/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/trainers/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/trainers/lightning_trainer.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/ui/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/ui/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    13646 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/ui/playground.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.955321 xturing-0.1.3/src/xturing/utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/utils/external_loggers.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/utils/hub.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/utils/interactive.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/utils/logging.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/utils/loss_fns.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/utils/notebooks.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/utils/text_splitter.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3803 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/utils/utils.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.923321 xturing-0.1.3/src/xturing.egg-info/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21623 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3201 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/SOURCES.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/dependency_links.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/entry_points.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/requires.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/top_level.txt
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.173109 xturing-0.1.4/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-06-13 13:40:44.000000 xturing-0.1.4/LICENSE
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-06-13 13:40:44.000000 xturing-0.1.4/MANIFEST.in
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-13 14:43:38.173109 xturing-0.1.4/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7359 2023-06-13 13:40:44.000000 xturing-0.1.4/README.md
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-06-13 13:40:45.000000 xturing-0.1.4/pyproject.toml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-06-13 14:43:38.173109 xturing-0.1.4/setup.cfg
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.149109 xturing-0.1.4/src/
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/__about__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/__init__.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing/cli/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/api.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/chat.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/ui.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing/config/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/config_data_classes.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3593 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/finetuning_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3090 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/generation_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1892 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/read_config.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/datasets/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8197 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/instruction_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/text2image_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/text_dataset.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/engines/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4033 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/bloom_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7209 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/cerebras_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/distilgpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2286 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/falcon_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/galactica_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1801 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/generic_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gptj_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/engines/gptj_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gptj_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gptj_utils/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6306 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/llama_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/engines/llama_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/llama_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    44506 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/llama_utils/llama.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/engines/lora_engine/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/lora.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/save_and_load.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/test.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/opt_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/engines/quant_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/quant_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8651 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/quant_utils/quant.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/model_apis/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/ai21.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/cohere.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/openai.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/models/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3290 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/bloom.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8363 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/cerebras.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/distilgpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1101 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/falcon.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/galactica.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1664 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/generic.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/gpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2259 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/llama.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/opt.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/stable_diffusion.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/preprocessors/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/instruction_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/text_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/registry.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/self_instruct/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/generate_instances.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/identify_if_classification.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/self_instruct/templates/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/trainers/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/trainers/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/trainers/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/trainers/lightning_trainer.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/ui/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/ui/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    13685 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/ui/playground.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.173109 xturing-0.1.4/src/xturing/utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/external_loggers.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/hub.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/interactive.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/logging.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/loss_fns.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/notebooks.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/text_splitter.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3803 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/utils.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing.egg-info/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3335 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/entry_points.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/requires.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.1.3/LICENSE` & `xturing-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/PKG-INFO` & `xturing-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -257,21 +257,19 @@
 - Scale from single to multiple GPUs for faster fine-tuning
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
-## 🌟 INT4 fine-tuning and generation with LLaMA LoRA
+## 🌟 What's new?
+We are excited to announce the latest enhancements to our `xTuring` library: Falcon LLM integration and Generic model support. With this update, you can use and finetune Falcon-7B model with the off-the-shelf, off-the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture with INT8 precision. Moreover, in case you do not find a model you want to run in the models' list, you can still us `xTuring` to run with the new `GenericModel` wrapper available to you. This new integration allows you to test and finetune any new model on xTuring without waiting for it to be integrated.
 
-We are excited to announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and generation integration. With this update, you can fine-tune LLMs like LLaMA with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This breakthrough significantly reduces memory requirements and accelerates the fine-tuning process, allowing you to achieve state-of-the-art performance with less computational resources.
-
-More information about INT4 fine-tuning and benchmarks can be found in the [INT4 README](examples/int4_finetuning/README.md).
-
-You can check out the [LLaMA INT4 fine-tuning example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
+You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
+Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
 
 <br>
 
 ## CLI playground
 <img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
 
 ## UI playground
@@ -371,14 +369,16 @@
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
+- [x] Support for a generic model wrapper
+- [x] Support for Falcon-7B model
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.3/README.md` & `xturing-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,21 +29,19 @@
 - Scale from single to multiple GPUs for faster fine-tuning
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
-## 🌟 INT4 fine-tuning and generation with LLaMA LoRA
+## 🌟 What's new?
+We are excited to announce the latest enhancements to our `xTuring` library: Falcon LLM integration and Generic model support. With this update, you can use and finetune Falcon-7B model with the off-the-shelf, off-the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture with INT8 precision. Moreover, in case you do not find a model you want to run in the models' list, you can still us `xTuring` to run with the new `GenericModel` wrapper available to you. This new integration allows you to test and finetune any new model on xTuring without waiting for it to be integrated.
 
-We are excited to announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and generation integration. With this update, you can fine-tune LLMs like LLaMA with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This breakthrough significantly reduces memory requirements and accelerates the fine-tuning process, allowing you to achieve state-of-the-art performance with less computational resources.
-
-More information about INT4 fine-tuning and benchmarks can be found in the [INT4 README](examples/int4_finetuning/README.md).
-
-You can check out the [LLaMA INT4 fine-tuning example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
+You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
+Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
 
 <br>
 
 ## CLI playground
 <img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
 
 ## UI playground
@@ -143,14 +141,16 @@
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
+- [x] Support for a generic model wrapper
+- [x] Support for Falcon-7B model
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

#### html2text {}

```diff
@@ -12,24 +12,26 @@
 computer or in your private cloud, ensuring data privacy and security. With
 `xTuring` you can, - Ingest data from different sources and preprocess them to
 a format LLMs can understand - Scale from single to multiple GPUs for faster
 fine-tuning - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning)
 to reduce hardware costs by up to 90% - Explore different fine-tuning methods
 and benchmark them to find the best performing model - Evaluate fine-tuned
 models on well-defined metrics for in-depth analysis
-## ð INT4 fine-tuning and generation with LLaMA LoRA We are excited to
-announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and
-generation integration. With this update, you can fine-tune LLMs like LLaMA
-with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This
-breakthrough significantly reduces memory requirements and accelerates the
-fine-tuning process, allowing you to achieve state-of-the-art performance with
-less computational resources. More information about INT4 fine-tuning and
-benchmarks can be found in the [INT4 README](examples/int4_finetuning/
-README.md). You can check out the [LLaMA INT4 fine-tuning example](examples/
-int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
+## ð What's new? We are excited to announce the latest enhancements to our
+`xTuring` library: Falcon LLM integration and Generic model support. With this
+update, you can use and finetune Falcon-7B model with the off-the-shelf, off-
+the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture
+with INT8 precision. Moreover, in case you do not find a model you want to run
+in the models' list, you can still us `xTuring` to run with the new
+`GenericModel` wrapper available to you. This new integration allows you to
+test and finetune any new model on xTuring without waiting for it to be
+integrated. You can check the [Falcon LoRA INT8 working example](examples/
+falcon/falcon_lora_int8.py) repository to see how it works. Also, you can check
+the [GenericModel working example](examples/generic/generic_model.py)
+repository to see how it works.
 ## CLI playground [.github/cli-playground.gif] ## UI playground [.github/ui-
 playground2.gif]
 ## âï¸ Installation ```bash pip install xturing ```
 ## ð Quickstart ```python from xturing.datasets import InstructionDataset
 from xturing.models import BaseModel # Load the dataset instruction_dataset =
 InstructionDataset("./alpaca_data") # Initialize the model model =
 BaseModel.create("llama_lora") # Finetune the model model.finetune
@@ -78,15 +80,16 @@
 llama_lora_finetuned_alpaca` |
 ## ð Roadmap - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT,
 Galactica and Bloom models - [x] Dataset generation using self-instruction -
 [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning - [x] INT8 low-
 precision fine-tuning support - [x] OpenAI, Cohere and AI21 Studio model APIs
 for dataset generation - [x] Added fine-tuned checkpoints for some models to
 the hub - [x] INT4 LLaMA LoRA fine-tuning demo - [x] INT4 LLaMA LoRA fine-
-tuning with INT4 generation - [ ] Evaluation of LLM models - [ ] Support for
+tuning with INT4 generation - [x] Support for a generic model wrapper - [x]
+Support for Falcon-7B model - [ ] Evaluation of LLM models - [ ] Support for
 Stable Diffusion
 ## ð¤ Help and Support If you have any questions, you can create an issue on
 this repository. You can also join our [Discord server](https://discord.gg/
 TgHXuSJEk6) and start a discussion in the `#xturing` channel.
 ## ð License This project is licensed under the Apache License 2.0 - see the
 [LICENSE](LICENSE) file for details.
 ## ð Contributing As an open source project in a rapidly evolving field, we
```

### Comparing `xturing-0.1.3/pyproject.toml` & `xturing-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.1.3"
+version = "0.1.4"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
```

### Comparing `xturing-0.1.3/src/xturing/cli/__init__.py` & `xturing-0.1.4/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/cli/api.py` & `xturing-0.1.4/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/cli/chat.py` & `xturing-0.1.4/src/xturing/cli/chat.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/config/__init__.py` & `xturing-0.1.4/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/config/config_data_classes.py` & `xturing-0.1.4/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.4/src/xturing/config/finetuning_config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -157,7 +157,62 @@
 
 bloom_lora_int8:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 8
   max_length: 256
+
+generic:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 8
+  max_length: 256
+
+generic_int8:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 8
+  max_length: 256
+
+generic_int8_lora:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 8
+  max_length: 256
+
+generic_lora:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 8
+  max_length: 256
+  
+falcon:
+  learning_rate: 5e-5
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 1
+  max_length: 256
+
+falcon_int8:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 1
+  max_length: 256
+
+falcon_lora:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 1
+
+falcon_lora_int8:
+  learning_rate: 1e-4
+  weight_decay: 0.01
+  num_train_epochs: 3
+  batch_size: 8
+  max_length: 256
```

### Comparing `xturing-0.1.3/src/xturing/config/generation_config.yaml` & `xturing-0.1.4/src/xturing/config/generation_config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -157,7 +157,48 @@
   max_new_tokens: 256
   do_sample: false
 
 # Greedy search
 bloom_lora_int8:
   max_new_tokens: 256
   do_sample: false
+
+# Greedy search
+generic:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+generic_int8:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+generic_lora:
+  max_new_tokens: 256
+  do_sample: false
+
+
+# Greedy search
+generic_lora_int8:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+falcon:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+falcon_lora:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+falcon_int8:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+falcon_lora_int8:
+  max_new_tokens: 256
+  do_sample: false
```

### Comparing `xturing-0.1.3/src/xturing/config/read_config.py` & `xturing-0.1.4/src/xturing/config/read_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 import yaml
 from pydantic import BaseModel
 
 
 def read_yaml(yml_path: Union[Path, str]):
     yml_path = str(yml_path)
@@ -27,28 +27,28 @@
     config.update(yml_content[model_name])
 
     config_object = data_class.parse_obj(config)
 
     return config_object
 
 
-def exists_xturing_config_file(dir_path: Union[Path, str] = None):
+def exists_xturing_config_file(dir_path: Optional[Union[Path, str]] = None):
     if dir_path is None:
         return False
     dir_path = Path(dir_path)
     assert dir_path.is_dir(), "The following path {} should be a directory".format(
         str(dir_path)
     )
 
     xturing_config_file_path = dir_path / "xturing.json"
 
     return xturing_config_file_path.is_file()
 
 
-def exists_lora_config_file(dir_path: Union[Path, str] = None):
+def exists_lora_config_file(dir_path: Optional[Union[Path, str]] = None):
     if dir_path is None:
         return False
     dir_path = Path(dir_path)
     assert dir_path.is_dir(), "The following path {} should be a directory".format(
         str(dir_path)
     )
```

### Comparing `xturing-0.1.3/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.4/src/xturing/datasets/instruction_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 class InstructionDataset(BaseDataset):
     config_name: str = "instruction_dataset"
 
     def __init__(
         self,
         path: Union[str, Path, HFDataset, dict],
         infix_instruction: bool = False,
-        promt_template: str = None,
+        promt_template: Optional[str] = None,
     ):
         if isinstance(path, HFDataset) or isinstance(path, DatasetDict):
             self.data = path
         elif isinstance(path, dict):
             self.data = {"train": HFDataset.from_dict(path)}
         else:
             path = Path(path)
```

### Comparing `xturing-0.1.3/src/xturing/datasets/text_dataset.py` & `xturing-0.1.4/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/__init__.py` & `xturing-0.1.4/src/xturing/engines/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,40 @@
 from .cerebras_engine import (
     CerebrasEngine,
     CerebrasInt8Engine,
     CerebrasLoraEngine,
     CerebrasLoraInt8Engine,
 )
 from .distilgpt2_engine import DistilGPT2Engine, DistilGPT2LoraEngine
+from .falcon_engine import (
+    FalconEngine,
+    FalconInt8Engine,
+    FalconLoraEngine,
+    FalconLoraInt8Engine,
+)
 from .galactica_engine import (
     GalacticaEngine,
     GalacticaInt8Engine,
     GalacticaLoraEngine,
     GalacticaLoraInt8Engine,
 )
+from .generic_engine import (
+    GenericEngine,
+    GenericInt8Engine,
+    GenericLoraEngine,
+    GenericLoraInt8Engine,
+)
 from .gpt2_engine import GPT2Engine, GPT2Int8Engine, GPT2LoraEngine, GPT2LoraInt8Engine
 from .gptj_engine import GPTJEngine, GPTJInt8Engine, GPTJLoraEngine, GPTJLoraInt8Engine
 from .llama_engine import (
     LLamaEngine,
     LLamaInt8Engine,
     LlamaLoraEngine,
-    LlamaLoraInt8Engine,
     LlamaLoraInt4Engine,
+    LlamaLoraInt8Engine,
 )
 from .opt_engine import OPTEngine, OPTInt8Engine, OPTLoraEngine, OPTLoraInt8Engine
 
 BaseEngine.add_to_registry(DistilGPT2Engine.config_name, DistilGPT2Engine)
 BaseEngine.add_to_registry(DistilGPT2LoraEngine.config_name, DistilGPT2LoraEngine)
 BaseEngine.add_to_registry(GPTJEngine.config_name, GPTJEngine)
 BaseEngine.add_to_registry(GPTJLoraEngine.config_name, GPTJLoraEngine)
@@ -56,7 +68,15 @@
 BaseEngine.add_to_registry(CerebrasLoraEngine.config_name, CerebrasLoraEngine)
 BaseEngine.add_to_registry(CerebrasInt8Engine.config_name, CerebrasInt8Engine)
 BaseEngine.add_to_registry(CerebrasLoraInt8Engine.config_name, CerebrasLoraInt8Engine)
 BaseEngine.add_to_registry(BloomEngine.config_name, BloomEngine)
 BaseEngine.add_to_registry(BloomLoraEngine.config_name, BloomLoraEngine)
 BaseEngine.add_to_registry(BloomInt8Engine.config_name, BloomInt8Engine)
 BaseEngine.add_to_registry(BloomLoraInt8Engine.config_name, BloomLoraInt8Engine)
+BaseEngine.add_to_registry(GenericEngine.config_name, GenericEngine)
+BaseEngine.add_to_registry(GenericInt8Engine.config_name, GenericInt8Engine)
+BaseEngine.add_to_registry(GenericLoraEngine.config_name, GenericLoraEngine)
+BaseEngine.add_to_registry(GenericLoraInt8Engine.config_name, GenericLoraInt8Engine)
+BaseEngine.add_to_registry(FalconEngine.config_name, FalconEngine)
+BaseEngine.add_to_registry(FalconLoraEngine.config_name, FalconLoraEngine)
+BaseEngine.add_to_registry(FalconInt8Engine.config_name, FalconInt8Engine)
+BaseEngine.add_to_registry(FalconLoraInt8Engine.config_name, FalconLoraInt8Engine)
```

### Comparing `xturing-0.1.3/src/xturing/engines/bloom_engine.py` & `xturing-0.1.4/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/causal.py` & `xturing-0.1.4/src/xturing/engines/causal.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,28 +25,30 @@
         self,
         *,
         model_name: Optional[str] = None,
         weights_path: Optional[Union[str, Path]] = None,
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
         load_8bit: Optional[bool] = False,
+        trust_remote_code: Optional[bool] = False,
     ):
         self.model_name = model_name
 
         if weights_path is not None:
             assert Path(
                 weights_path
             ).is_dir(), "The weights path should be a existing directory"
             if load_8bit:
                 device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
                 self.model = AutoModelForCausalLM.from_pretrained(
                     weights_path,
                     torch_dtype=DEFAULT_DTYPE,
                     load_in_8bit=True,
                     device_map=device_map,
+                    trust_remote_code=trust_remote_code,
                 )
                 self.model = prepare_model_for_int8_training(self.model)
             else:
                 self.model = AutoModelForCausalLM.from_pretrained(
                     weights_path, torch_dtype=DEFAULT_DTYPE
                 )
             self.tokenizer = AutoTokenizer.from_pretrained(weights_path)
@@ -57,21 +59,24 @@
             if load_8bit:
                 device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
                 self.model = AutoModelForCausalLM.from_pretrained(
                     model_name,
                     torch_dtype=DEFAULT_DTYPE,
                     load_in_8bit=True,
                     device_map=device_map,
+                    trust_remote_code=trust_remote_code,
                 )
                 for param in self.model.parameters():
                     param.data = param.data.contiguous()
                 self.model = prepare_model_for_int8_training(self.model)
             else:
                 self.model = AutoModelForCausalLM.from_pretrained(
-                    model_name, torch_dtype=DEFAULT_DTYPE
+                    model_name,
+                    torch_dtype=DEFAULT_DTYPE,
+                    trust_remote_code=trust_remote_code,
                 )
             self.tokenizer = AutoTokenizer.from_pretrained(model_name)
         else:
             raise ValueError(
                 "Please provide a model_name, the weights path or model and tokenizer."
             )
 
@@ -124,25 +129,27 @@
         *,
         model_name: Optional[str] = None,
         weights_path: Optional[Union[str, Path]] = None,
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
         load_8bit: Optional[bool] = False,
         target_modules: Optional[Union[List[str], str]] = None,
+        trust_remote_code: Optional[bool] = False,
     ):
         # The base model should always be loaded from the original model
         # That's why weights_path is None. If not model.eval() will fail later
         super().__init__(
             model_name=model_name,
             weights_path=None
             if exists_xturing_config_file(weights_path)
             else weights_path,
             model=model,
             tokenizer=tokenizer,
             load_8bit=load_8bit,
+            trust_remote_code=trust_remote_code,
         )
 
         # The model before applying LoRA
         self.base_model = self.model
 
         lora_config = LoraConfig(
             r=8,
```

### Comparing `xturing-0.1.3/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.4/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.4/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/galactica_engine.py` & `xturing-0.1.4/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.4/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/gptj_engine.py` & `xturing-0.1.4/src/xturing/engines/gptj_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.4/src/xturing/engines/gptj_utils/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/llama_engine.py` & `xturing-0.1.4/src/xturing/engines/llama_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.4/src/xturing/engines/llama_utils/llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -753,15 +753,15 @@
                 else expanded_attn_mask + combined_attention_mask
             )
 
         return combined_attention_mask
 
     def forward(
         self,
-        input_ids: torch.LongTensor = None,
+        input_ids: Optional[torch.LongTensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         past_key_values: Optional[List[torch.FloatTensor]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
@@ -959,15 +959,15 @@
         self.model = decoder
 
     def get_decoder(self):
         return self.model
 
     def forward(
         self,
-        input_ids: torch.LongTensor = None,
+        input_ids: Optional[torch.LongTensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         past_key_values: Optional[List[torch.FloatTensor]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
         labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
```

### Comparing `xturing-0.1.3/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.4/src/xturing/engines/lora_engine/lora.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/lora_engine/save_and_load.py` & `xturing-0.1.4/src/xturing/engines/lora_engine/save_and_load.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/opt_engine.py` & `xturing-0.1.4/src/xturing/engines/opt_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/engines/quant_utils/quant.py` & `xturing-0.1.4/src/xturing/engines/quant_utils/quant.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/model_apis/__init__.py` & `xturing-0.1.4/src/xturing/model_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/model_apis/ai21.py` & `xturing-0.1.4/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/model_apis/base.py` & `xturing-0.1.4/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/model_apis/cohere.py` & `xturing-0.1.4/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/model_apis/openai.py` & `xturing-0.1.4/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/__init__.py` & `xturing-0.1.4/src/xturing/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from .base import BaseModel
 from .bloom import Bloom, BloomInt8, BloomLora, BloomLoraInt8
 from .cerebras import Cerebras, CerebrasInt8, CerebrasLora, CerebrasLoraInt8
 from .distilgpt2 import DistilGPT2, DistilGPT2Lora
+from .falcon import Falcon, FalconInt8, FalconLora, FalconLoraInt8
 from .galactica import Galactica, GalacticaInt8, GalacticaLora, GalacticaLoraInt8
+from .generic import (
+    GenericInt8Model,
+    GenericLoraInt8Model,
+    GenericLoraModel,
+    GenericModel,
+)
 from .gpt2 import GPT2, GPT2Int8, GPT2Lora, GPT2LoraInt8
 from .gptj import GPTJ, GPTJInt8, GPTJLora, GPTJLoraInt8
-from .llama import Llama, LlamaInt8, LlamaLora, LlamaLoraInt8, LlamaLoraInt4
+from .llama import Llama, LlamaInt8, LlamaLora, LlamaLoraInt4, LlamaLoraInt8
 from .opt import OPT, OPTInt8, OPTLora, OPTLoraInt8
 from .stable_diffusion import StableDiffusion
 
 BaseModel.add_to_registry(DistilGPT2.config_name, DistilGPT2)
 BaseModel.add_to_registry(DistilGPT2Lora.config_name, DistilGPT2Lora)
 BaseModel.add_to_registry(GPT2.config_name, GPT2)
 BaseModel.add_to_registry(GPT2Lora.config_name, GPT2Lora)
@@ -37,7 +44,15 @@
 BaseModel.add_to_registry(CerebrasInt8.config_name, CerebrasInt8)
 BaseModel.add_to_registry(CerebrasLoraInt8.config_name, CerebrasLoraInt8)
 BaseModel.add_to_registry(Bloom.config_name, Bloom)
 BaseModel.add_to_registry(BloomLora.config_name, BloomLora)
 BaseModel.add_to_registry(BloomInt8.config_name, BloomInt8)
 BaseModel.add_to_registry(BloomLoraInt8.config_name, BloomLoraInt8)
 BaseModel.add_to_registry(StableDiffusion.config_name, StableDiffusion)
+BaseModel.add_to_registry(GenericModel.config_name, GenericModel)
+BaseModel.add_to_registry(GenericLoraModel.config_name, GenericLoraModel)
+BaseModel.add_to_registry(GenericInt8Model.config_name, GenericInt8Model)
+BaseModel.add_to_registry(GenericLoraInt8Model.config_name, GenericLoraInt8Model)
+BaseModel.add_to_registry(Falcon.config_name, Falcon)
+BaseModel.add_to_registry(FalconLora.config_name, FalconLora)
+BaseModel.add_to_registry(FalconInt8.config_name, FalconInt8)
+BaseModel.add_to_registry(FalconLoraInt8.config_name, FalconLoraInt8)
```

### Comparing `xturing-0.1.3/src/xturing/models/base.py` & `xturing-0.1.4/src/xturing/models/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/bloom.py` & `xturing-0.1.4/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/causal.py` & `xturing-0.1.4/src/xturing/models/causal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from pathlib import Path
-from typing import Iterable, List, Optional, Union, Type
+from typing import Iterable, List, Optional, Type, Union
 
 import torch
+from pytorch_lightning.loggers import Logger
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from xturing.config import DEFAULT_DEVICE, assert_not_cpu_int8
 from xturing.config.config_data_classes import FinetuningConfig, GenerationConfig
 from xturing.config.read_config import load_config
 from xturing.datasets.instruction_dataset import InstructionDataset
@@ -14,35 +15,46 @@
 from xturing.engines.base import BaseEngine
 from xturing.engines.causal import CausalLoraEngine
 from xturing.models import BaseModel
 from xturing.preprocessors.base import BasePreprocessor
 from xturing.trainers.base import BaseTrainer
 from xturing.trainers.lightning_trainer import LightningTrainer
 from xturing.utils.logging import configure_logger
-from pytorch_lightning.loggers import Logger
 
 logger = configure_logger(__name__)
 
 
 class CausalModel(BaseModel):
-    def __init__(self, engine: str, weights_path: Optional[str] = None):
-        self.engine = BaseEngine.create(engine, weights_path)
+    def __init__(
+        self,
+        engine: str,
+        weights_path: Optional[str] = None,
+        model_name: Optional[str] = None,
+        target_modules: Optional[List[str]] = None,
+    ):
+        self.engine = BaseEngine.create(
+            engine,
+            weights_path=weights_path,
+            model_name=model_name,
+            target_modules=target_modules,
+        )
 
         self.model_name = engine.replace("_engine", "")
 
         # Finetuning config
         self.finetuning_args = load_config(
             model_name=self.model_name,
             config_path=Path(__file__).parent.parent
             / "config"
             / "finetuning_config.yaml",
             data_class=FinetuningConfig,
         )
 
         # Generation config
+
         self.generation_args = load_config(
             model_name=engine.replace("_engine", ""),
             config_path=Path(__file__).parent.parent
             / "config"
             / "generation_config.yaml",
             data_class=GenerationConfig,
         )
@@ -60,30 +72,36 @@
         return BasePreprocessor.create(
             dataset.config_name,
             self.engine.tokenizer,
             int(self.finetuning_args.max_length),
             dataset.meta,
         )
 
-    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset], 
-                      logger: Union[Logger, Iterable[Logger], bool] = True):
+    def _make_trainer(
+        self,
+        dataset: Union[TextDataset, InstructionDataset],
+        logger: Union[Logger, Iterable[Logger], bool] = True,
+    ):
         return BaseTrainer.create(
             LightningTrainer.config_name,
             self.engine,
             dataset,
             self._make_collate_fn(dataset),
             int(self.finetuning_args.num_train_epochs),
             int(self.finetuning_args.batch_size),
             float(self.finetuning_args.learning_rate),
             self.finetuning_args.optimizer_name,
             logger=logger,
         )
 
-    def finetune(self, dataset: Union[TextDataset, InstructionDataset], 
-                 logger: Union[Logger, Iterable[Logger], bool] = True):
+    def finetune(
+        self,
+        dataset: Union[TextDataset, InstructionDataset],
+        logger: Union[Logger, Iterable[Logger], bool] = True,
+    ):
         assert dataset.config_name in [
             "text_dataset",
             "instruction_dataset",
         ], "Please make sure the dataset_type is text_dataset or instruction_dataset"
         trainer = self._make_trainer(dataset, logger)
         trainer.fit()
 
@@ -179,25 +197,44 @@
             path.mkdir(parents=True, exist_ok=True)
 
         self.engine.save(path)
         self._save_config(path=path)
 
 
 class CausalInt8Model(CausalModel):
-    def __init__(self, engine: str, weights_path: Optional[str] = None):
+    def __init__(
+        self,
+        engine: str,
+        weights_path: Optional[str] = None,
+        model_name: Optional[str] = None,
+    ):
         assert_not_cpu_int8()
-        super().__init__(engine, weights_path)
+        super().__init__(engine, weights_path=weights_path, model_name=model_name)
 
 
 class CausalLoraModel(CausalModel):
-    def __init__(self, engine: str, weights_path: Optional[str] = None):
-        super().__init__(engine, weights_path)
+    def __init__(
+        self,
+        engine: str,
+        weights_path: Optional[str] = None,
+        model_name: Optional[str] = None,
+        target_modules: Optional[List[str]] = None,
+    ):
+        super().__init__(
+            engine,
+            weights_path=weights_path,
+            model_name=model_name,
+            target_modules=target_modules,
+        )
 
-    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset], 
-                      logger: Union[Logger, Iterable[Logger], bool] = True):
+    def _make_trainer(
+        self,
+        dataset: Union[TextDataset, InstructionDataset],
+        logger: Union[Logger, Iterable[Logger], bool] = True,
+    ):
         return BaseTrainer.create(
             LightningTrainer.config_name,
             self.engine,
             dataset,
             self._make_collate_fn(dataset),
             int(self.finetuning_args.num_train_epochs),
             int(self.finetuning_args.batch_size),
@@ -206,10 +243,21 @@
             True,
             True,
             logger=logger,
         )
 
 
 class CausalLoraInt8Model(CausalLoraModel):
-    def __init__(self, engine: str, weights_path: Optional[str] = None):
+    def __init__(
+        self,
+        engine: str,
+        weights_path: Optional[str] = None,
+        model_name: Optional[str] = None,
+        target_modules: Optional[List[str]] = None,
+    ):
         assert_not_cpu_int8()
-        super().__init__(engine, weights_path)
+        super().__init__(
+            engine,
+            weights_path=weights_path,
+            model_name=model_name,
+            target_modules=target_modules,
+        )
```

### Comparing `xturing-0.1.3/src/xturing/models/cerebras.py` & `xturing-0.1.4/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/distilgpt2.py` & `xturing-0.1.4/src/xturing/models/distilgpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/galactica.py` & `xturing-0.1.4/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/gpt2.py` & `xturing-0.1.4/src/xturing/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/gptj.py` & `xturing-0.1.4/src/xturing/models/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/llama.py` & `xturing-0.1.4/src/xturing/models/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/opt.py` & `xturing-0.1.4/src/xturing/models/opt.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/models/stable_diffusion.py` & `xturing-0.1.4/src/xturing/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.4/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.4/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/registry.py` & `xturing-0.1.4/src/xturing/registry.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.4/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.4/src/xturing/self_instruct/generate_instances.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.4/src/xturing/self_instruct/identify_if_classification.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.4/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.4/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.4/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.4/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.4/src/xturing/trainers/lightning_trainer.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/ui/playground.py` & `xturing-0.1.4/src/xturing/ui/playground.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import Optional
+
 import gradio as gr
 
 from xturing.models.base import BaseModel
 
 model_to_class_map = {"GPT-2": "gpt2", "GPT-J": "gptj", "Llama": "llama"}
 
 
 class Playground:
     def __init__(
         self,
-        model_path: str = None,
+        model_path: Optional[str] = None,
     ):
         self.penalty_alpha = None
         self.top_k = None
         self.top_p = 0.92
         self.do_sample = True
         self.max_new_tokens = 256
```

### Comparing `xturing-0.1.3/src/xturing/utils/hub.py` & `xturing-0.1.4/src/xturing/utils/hub.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/utils/logging.py` & `xturing-0.1.4/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/utils/loss_fns.py` & `xturing-0.1.4/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/utils/notebooks.py` & `xturing-0.1.4/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/utils/text_splitter.py` & `xturing-0.1.4/src/xturing/utils/text_splitter.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing/utils/utils.py` & `xturing-0.1.4/src/xturing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.3/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.4/src/xturing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -257,21 +257,19 @@
 - Scale from single to multiple GPUs for faster fine-tuning
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
-## 🌟 INT4 fine-tuning and generation with LLaMA LoRA
+## 🌟 What's new?
+We are excited to announce the latest enhancements to our `xTuring` library: Falcon LLM integration and Generic model support. With this update, you can use and finetune Falcon-7B model with the off-the-shelf, off-the-shelf with INT8 precision, with LoRA architecture, and LoRA architecture with INT8 precision. Moreover, in case you do not find a model you want to run in the models' list, you can still us `xTuring` to run with the new `GenericModel` wrapper available to you. This new integration allows you to test and finetune any new model on xTuring without waiting for it to be integrated.
 
-We are excited to announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and generation integration. With this update, you can fine-tune LLMs like LLaMA with LoRA architecture in INT4 precision with less than `6 GB` of VRAM. This breakthrough significantly reduces memory requirements and accelerates the fine-tuning process, allowing you to achieve state-of-the-art performance with less computational resources.
-
-More information about INT4 fine-tuning and benchmarks can be found in the [INT4 README](examples/int4_finetuning/README.md).
-
-You can check out the [LLaMA INT4 fine-tuning example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) to see how it works.
+You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
+Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
 
 <br>
 
 ## CLI playground
 <img src=".github/cli-playground.gif" width="100%" style="margin: 0 1%;"/>
 
 ## UI playground
@@ -371,14 +369,16 @@
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
+- [x] Support for a generic model wrapper
+- [x] Support for Falcon-7B model
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.3/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.4/src/xturing.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 src/xturing/datasets/text_dataset.py
 src/xturing/engines/__init__.py
 src/xturing/engines/base.py
 src/xturing/engines/bloom_engine.py
 src/xturing/engines/causal.py
 src/xturing/engines/cerebras_engine.py
 src/xturing/engines/distilgpt2_engine.py
+src/xturing/engines/falcon_engine.py
 src/xturing/engines/galactica_engine.py
+src/xturing/engines/generic_engine.py
 src/xturing/engines/gpt2_engine.py
 src/xturing/engines/gptj_engine.py
 src/xturing/engines/llama_engine.py
 src/xturing/engines/opt_engine.py
 src/xturing/engines/gptj_utils/__init__.py
 src/xturing/engines/gptj_utils/gptj.py
 src/xturing/engines/llama_utils/__init__.py
@@ -54,15 +56,17 @@
 src/xturing/model_apis/openai.py
 src/xturing/models/__init__.py
 src/xturing/models/base.py
 src/xturing/models/bloom.py
 src/xturing/models/causal.py
 src/xturing/models/cerebras.py
 src/xturing/models/distilgpt2.py
+src/xturing/models/falcon.py
 src/xturing/models/galactica.py
+src/xturing/models/generic.py
 src/xturing/models/gpt2.py
 src/xturing/models/gptj.py
 src/xturing/models/llama.py
 src/xturing/models/opt.py
 src/xturing/models/stable_diffusion.py
 src/xturing/preprocessors/__init__.py
 src/xturing/preprocessors/base.py
```

