# Comparing `tmp/flagai-1.7.1.tar.gz` & `tmp/flagai-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagai-1.7.1.tar", last modified: Sat Jun 10 13:58:22 2023, max compression
+gzip compressed data, was "flagai-1.7.2.tar", last modified: Tue Jun 13 09:35:24 2023, max compression
```

## Comparing `flagai-1.7.1.tar` & `flagai-1.7.2.tar`

### file list

```diff
@@ -1,311 +1,328 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.220402 flagai-1.7.1/
--rwxr-xr-x   0 root         (0) root         (0)    10219 2023-06-10 13:56:07.000000 flagai-1.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    20120 2023-06-10 13:58:22.220402 flagai-1.7.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    19744 2023-06-10 13:56:07.000000 flagai-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.196402 flagai-1.7.1/flagai/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.196402 flagai-1.7.1/flagai/auto_model/
--rwxr-xr-x   0 root         (0) root         (0)       27 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/auto_model/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14985 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/auto_model/auto_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4025 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/collate_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/
--rwxr-xr-x   0 root         (0) root         (0)      400 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/block/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/block/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27923 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/block/blocklm_utils.py
--rw-r--r--   0 root         (0) root         (0)     6750 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/block/corpora.py
--rw-r--r--   0 root         (0) root         (0)     6395 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/block/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     7270 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/block/dataset.py
--rw-r--r--   0 root         (0) root         (0)    10141 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/block/lazy_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/cpm3_data/
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/cpm3_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2660 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/cpm3_data/dataset.py
--rw-r--r--   0 root         (0) root         (0)     6262 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/cpm3_data/distributed_indexed.py
--rw-r--r--   0 root         (0) root         (0)     4531 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/cpm3_data/indexed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/data_collator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/data_collator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38469 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/data_collator/collate_fn.py
--rwxr-xr-x   0 root         (0) root         (0)    13797 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/data_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/indexed_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/indexed_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15072 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/indexed_dataset/build_datasets.py
--rwxr-xr-x   0 root         (0) root         (0)    23076 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/indexed_dataset/build_index_mappings.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/indexed_dataset/check_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/indexed_dataset/merge_datasets.py
--rw-r--r--   0 root         (0) root         (0)     8738 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/dataset/indexed_dataset/preprocess_data_args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/language_model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/language_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12850 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/language_model/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/mm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/mm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/mm/clip_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/seq2seq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/seq2seq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28134 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/seq2seq/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/dataset/superglue/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/superglue/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9434 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/superglue/control.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/superglue/dataset.py
--rw-r--r--   0 root         (0) root         (0)    64586 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/superglue/processor.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/superglue/properties.py
--rw-r--r--   0 root         (0) root         (0)    64718 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/dataset/superglue/pvp.py
--rwxr-xr-x   0 root         (0) root         (0)     8550 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/file_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/tokenizer/
--rwxr-xr-x   0 root         (0) root         (0)      628 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.200402 flagai-1.7.1/flagai/data/tokenizer/bert/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/bert/bert_tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    24023 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/bert/wordpiece.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/clip/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6261 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/clip/tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/cpm_1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/cpm_1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3845 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/cpm_1/cpm1_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/cpm_3/
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/cpm_3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9267 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/cpm_3/cpm3_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/galactica/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/galactica/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3167 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/galactica/galactica_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/glm_10b_en/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_10b_en/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12263 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_10b_en/glm_10b_en_bpe_tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    14814 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_10b_en/glm_10b_en_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/glm_large_ch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_large_ch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5250 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_large_ch/glm_large_ch.py
--rw-r--r--   0 root         (0) root         (0)    10378 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_large_ch/glm_large_ch_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/glm_large_en/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_large_en/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7982 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_large_en/glm_large_en_tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    13641 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/glm_large_en/wordpiece.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/llama/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/llama/tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/opt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/opt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5003 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/opt/opt_en_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/roberta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4930 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/roberta/roberta_tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/t5/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/t5/t5_pegasus_tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    17572 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/data/tokenizer/t5/t5_tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)    18924 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/tokenizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5450 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/base_tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)    12990 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/bpe_tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)    16106 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/diffusion_bert_tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)      242 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/properties.py
--rwxr-xr-x   0 root         (0) root         (0)     2572 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/sp_tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)    35838 2023-06-10 13:56:17.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)    13383 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/wp_tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)    16865 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/data/tokenizer/wp_tokenizer.py
--rwxr-xr-x   0 root         (0) root         (0)    13407 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/env_args.py
--rwxr-xr-x   0 root         (0) root         (0)    45953 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/env_trainer.py
--rwxr-xr-x   0 root         (0) root         (0)    53952 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/env_trainer_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.204402 flagai-1.7.1/flagai/fp16/
--rwxr-xr-x   0 root         (0) root         (0)      941 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/fp16/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32292 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/fp16/fp16.py
--rwxr-xr-x   0 root         (0) root         (0)     8015 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/fp16/fp16util.py
--rwxr-xr-x   0 root         (0) root         (0)     8317 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/fp16/loss_scaler.py
--rwxr-xr-x   0 root         (0) root         (0)     9467 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/launch.py
--rwxr-xr-x   0 root         (0) root         (0)     3930 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/logger.py
--rwxr-xr-x   0 root         (0) root         (0)     5303 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.208402 flagai-1.7.1/flagai/model/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      140 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/alm_model.py
--rwxr-xr-x   0 root         (0) root         (0)    11506 2023-06-10 13:56:17.000000 flagai-1.7.1/flagai/model/aquila_model.py
--rwxr-xr-x   0 root         (0) root         (0)    12548 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/base_model.py
--rwxr-xr-x   0 root         (0) root         (0)    24995 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/bert_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.208402 flagai-1.7.1/flagai/model/blocks/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/blocks/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2169 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/blocks/aquila_block.py
--rwxr-xr-x   0 root         (0) root         (0)     4926 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/blocks/bert_block.py
--rwxr-xr-x   0 root         (0) root         (0)    15383 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/blocks/cpm_block.py
--rwxr-xr-x   0 root         (0) root         (0)     9222 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/blocks/glm_block.py
--rwxr-xr-x   0 root         (0) root         (0)     2290 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/blocks/gpt2_block.py
--rwxr-xr-x   0 root         (0) root         (0)     5307 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/blocks/t5_block.py
--rwxr-xr-x   0 root         (0) root         (0)     1517 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/config.py
--rwxr-xr-x   0 root         (0) root         (0)    19137 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/cpm3_model.py
--rwxr-xr-x   0 root         (0) root         (0)    16321 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/cpm3_train_model.py
--rwxr-xr-x   0 root         (0) root         (0)       75 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/cpm_model.py
--rwxr-xr-x   0 root         (0) root         (0)     5656 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     7998 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/galactica_model.py
--rwxr-xr-x   0 root         (0) root         (0)    40848 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/glm_model.py
--rwxr-xr-x   0 root         (0) root         (0)    15226 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/gpt2_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.208402 flagai-1.7.1/flagai/model/layers/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7112 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/activations.py
--rwxr-xr-x   0 root         (0) root         (0)    73399 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/attentions.py
--rwxr-xr-x   0 root         (0) root         (0)    18699 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/attentions_bmt.py
--rwxr-xr-x   0 root         (0) root         (0)     3063 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/crf.py
--rwxr-xr-x   0 root         (0) root         (0)    21600 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/embeddings.py
--rwxr-xr-x   0 root         (0) root         (0)     9666 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/embeddings_bmt.py
--rwxr-xr-x   0 root         (0) root         (0)    27514 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/feedforward.py
--rwxr-xr-x   0 root         (0) root         (0)    10505 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/feedforward_bmt.py
--rwxr-xr-x   0 root         (0) root         (0)     4034 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/global_pointer.py
--rwxr-xr-x   0 root         (0) root         (0)     4316 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/layer_norm.py
--rwxr-xr-x   0 root         (0) root         (0)     2269 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/layer_norm_bmt.py
--rwxr-xr-x   0 root         (0) root         (0)     2659 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/linear.py
--rwxr-xr-x   0 root         (0) root         (0)     2959 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/layers/linear_bmt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/
--rwxr-xr-x   0 root         (0) root         (0)    18852 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/AltCLIP.py
--rwxr-xr-x   0 root         (0) root         (0)    81528 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/AltDiffusion.py
--rwxr-xr-x   0 root         (0) root         (0)    85758 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/AltDiffusionM18.py
--rwxr-xr-x   0 root         (0) root         (0)    25335 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/Sampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/Unets/
--rw-r--r--   0 root         (0) root         (0)    35142 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/Unets/Unet.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/Unets/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/attentions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/attentions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8517 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/attentions/attention.py
--rwxr-xr-x   0 root         (0) root         (0)     8609 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/autoencoder_m18.py
--rwxr-xr-x   0 root         (0) root         (0)    18905 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/autoencoders.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/clip_guohua/
--rw-r--r--   0 root         (0) root         (0)       74 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/clip_guohua/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14839 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/clip_guohua/bert_tokenizer.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/clip_guohua/clip.py
--rw-r--r--   0 root         (0) root         (0)     3905 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/clip_guohua/configuration_bert.py
--rw-r--r--   0 root         (0) root         (0)    18569 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/clip_guohua/model.py
--rw-r--r--   0 root         (0) root         (0)    20144 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/clip_guohua/modeling_bert.py
--rwxr-xr-x   0 root         (0) root         (0)    12489 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/clip_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/dpm_solver/
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/dpm_solver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65969 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/dpm_solver/dpm_solver.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/dpm_solver/sampler.py
--rwxr-xr-x   0 root         (0) root         (0)    24330 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/eva_clip_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/lm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/lm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2083 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/lm/clip_guohua.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/lm/dcn_clip.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/lm/en_clip.py
--rw-r--r--   0 root         (0) root         (0)    20168 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/lm/x_transformer.py
--rwxr-xr-x   0 root         (0) root         (0)    38506 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/model.py
--rwxr-xr-x   0 root         (0) root         (0)    67851 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/modeling_altclip.py
--rwxr-xr-x   0 root         (0) root         (0)     5632 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/modeling_berts.py
--rwxr-xr-x   0 root         (0) root         (0)     6277 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/modeling_berts_m18.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11904 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/attention.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34396 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/model.py
--rw-r--r--   0 root         (0) root         (0)    35811 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 root         (0) root         (0)     9881 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/mm/modules/distributions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/distributions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2970 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/distributions/distributions.py
--rw-r--r--   0 root         (0) root         (0)     3229 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/mm/modules/ema.py
--rwxr-xr-x   0 root         (0) root         (0)    21130 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/mm/utils.py
--rwxr-xr-x   0 root         (0) root         (0)     8308 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/opt_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.212402 flagai-1.7.1/flagai/model/predictor/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/predictor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6338 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/predictor/aquila.py
--rwxr-xr-x   0 root         (0) root         (0)     2614 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/predictor/gpt.py
--rwxr-xr-x   0 root         (0) root         (0)    23307 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/predictor/predictor.py
--rwxr-xr-x   0 root         (0) root         (0)     5315 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/predictor/simctg.py
--rwxr-xr-x   0 root         (0) root         (0)    91302 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/predictor/utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2561 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/prompt.py
--rwxr-xr-x   0 root         (0) root         (0)    57714 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/t5_model.py
--rwxr-xr-x   0 root         (0) root         (0)     2370 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.216402 flagai-1.7.1/flagai/model/vision/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/vision/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2857 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/vision/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.220402 flagai-1.7.1/flagai/model/vision/layers/
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4040 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/activations.py
--rw-r--r--   0 root         (0) root         (0)     2529 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/activations_jit.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/activations_me.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/adaptive_avgmax_pool.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/attention_pool2d.py
--rw-r--r--   0 root         (0) root         (0)     1594 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/blur_pool.py
--rw-r--r--   0 root         (0) root         (0)     6895 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/bottleneck_attn.py
--rw-r--r--   0 root         (0) root         (0)     4426 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/cbam.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/classifier.py
--rw-r--r--   0 root         (0) root         (0)     5199 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/cond_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/config.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/conv2d_same.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/conv_bn_act.py
--rw-r--r--   0 root         (0) root         (0)     5104 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/create_act.py
--rw-r--r--   0 root         (0) root         (0)     3526 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/create_attn.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/create_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     3562 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/create_norm_act.py
--rw-r--r--   0 root         (0) root         (0)     6786 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/drop.py
--rw-r--r--   0 root         (0) root         (0)     6386 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/eca.py
--rw-r--r--   0 root         (0) root         (0)    13792 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/evo_norm.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/filter_response_norm.py
--rw-r--r--   0 root         (0) root         (0)     3824 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/gather_excite.py
--rw-r--r--   0 root         (0) root         (0)     2445 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/global_context.py
--rw-r--r--   0 root         (0) root         (0)    10662 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/halo_attn.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/inplace_abn.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/lambda_layer.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/linear.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/median_pool.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/mixed_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     7008 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/ml_decoder.py
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/mlp.py
--rw-r--r--   0 root         (0) root         (0)     6218 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/non_local_attn.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/norm.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/norm_act.py
--rw-r--r--   0 root         (0) root         (0)     2167 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/padding.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/patch_embed.py
--rw-r--r--   0 root         (0) root         (0)     3045 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/pool2d_same.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/pos_embed.py
--rw-r--r--   0 root         (0) root         (0)     5387 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/selective_kernel.py
--rw-r--r--   0 root         (0) root         (0)     2620 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/separable_conv.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/space_to_depth.py
--rw-r--r--   0 root         (0) root         (0)     3076 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/split_attn.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/split_batchnorm.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/squeeze_excite.py
--rw-r--r--   0 root         (0) root         (0)     5887 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/std_conv.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/test_time_pool.py
--rw-r--r--   0 root         (0) root         (0)      335 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/trace_utils.py
--rw-r--r--   0 root         (0) root         (0)     3265 2023-06-10 05:30:57.000000 flagai-1.7.1/flagai/model/vision/layers/weight_init.py
--rwxr-xr-x   0 root         (0) root         (0)    28804 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/vision/swinv1.py
--rwxr-xr-x   0 root         (0) root         (0)    29099 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/vision/swinv2.py
--rwxr-xr-x   0 root         (0) root         (0)    23433 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/model/vision/vit.py
--rwxr-xr-x   0 root         (0) root         (0)    16329 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mp_tools.py
--rwxr-xr-x   0 root         (0) root         (0)     7391 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mp_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.220402 flagai-1.7.1/flagai/mpu/
--rwxr-xr-x   0 root         (0) root         (0)     1637 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4952 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/cross_entropy.py
--rwxr-xr-x   0 root         (0) root         (0)     4143 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/data.py
--rwxr-xr-x   0 root         (0) root         (0)     1509 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/func_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     3123 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/grads.py
--rwxr-xr-x   0 root         (0) root         (0)     4973 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/initialize.py
--rwxr-xr-x   0 root         (0) root         (0)     2287 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/local_attention_function.py
--rwxr-xr-x   0 root         (0) root         (0)     4254 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/mappings.py
--rwxr-xr-x   0 root         (0) root         (0)    14979 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/random.py
--rwxr-xr-x   0 root         (0) root         (0)     2899 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/mpu/utils.py
--rwxr-xr-x   0 root         (0) root         (0)     5772 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/optimizers.py
--rwxr-xr-x   0 root         (0) root         (0)     6043 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/schedulers.py
--rwxr-xr-x   0 root         (0) root         (0)     5616 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/test_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    50816 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/trainer.py
--rwxr-xr-x   0 root         (0) root         (0)    60172 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/trainer_v1.py
--rwxr-xr-x   0 root         (0) root         (0)    12428 2023-06-10 13:56:07.000000 flagai-1.7.1/flagai/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.196402 flagai-1.7.1/flagai.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20120 2023-06-10 13:58:21.000000 flagai-1.7.1/flagai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9580 2023-06-10 13:58:22.000000 flagai-1.7.1/flagai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 13:58:21.000000 flagai-1.7.1/flagai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      342 2023-06-10 13:58:21.000000 flagai-1.7.1/flagai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-10 13:58:21.000000 flagai-1.7.1/flagai.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      106 2023-06-10 13:58:22.220402 flagai-1.7.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1310 2023-06-10 13:57:15.000000 flagai-1.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:58:22.220402 flagai-1.7.1/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3645 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/bak_test_superglue.py
--rwxr-xr-x   0 root         (0) root         (0)     1538 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/bak_test_t5_ch.py
--rwxr-xr-x   0 root         (0) root         (0)     5251 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/test_autoloader.py
--rwxr-xr-x   0 root         (0) root         (0)     2500 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/test_bert.py
--rwxr-xr-x   0 root         (0) root         (0)     1399 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/test_glm_large_ch.py
--rwxr-xr-x   0 root         (0) root         (0)     2755 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/test_glm_seq2seq.py
--rwxr-xr-x   0 root         (0) root         (0)     1009 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/test_gpt2_ch.py
--rwxr-xr-x   0 root         (0) root         (0)    11246 2023-06-10 13:56:07.000000 flagai-1.7.1/tests/test_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.179077 flagai-1.7.2/
+-rwxrwxrwx   0 root         (0) root         (0)    10219 2023-06-13 05:25:15.000000 flagai-1.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20437 2023-06-13 09:35:24.179077 flagai-1.7.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    20041 2023-06-13 08:29:18.000000 flagai-1.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai/auto_model/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/auto_model/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14914 2023-06-13 07:15:18.000000 flagai-1.7.2/flagai/auto_model/auto_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4025 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/collate_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai/data/dataset/
+-rwxrwxrwx   0 root         (0) root         (0)      400 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai/data/dataset/block/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/block/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27923 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/block/blocklm_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6750 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/block/corpora.py
+-rw-r--r--   0 root         (0) root         (0)     6395 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/block/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/block/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10141 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/block/lazy_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai/data/dataset/cpm3_data/
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/cpm3_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/cpm3_data/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6262 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/cpm3_data/distributed_indexed.py
+-rw-r--r--   0 root         (0) root         (0)     4531 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/cpm3_data/indexed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai/data/dataset/data_collator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/data_collator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38469 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/data_collator/collate_fn.py
+-rwxrwxrwx   0 root         (0) root         (0)    13797 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/data_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/dataset/indexed_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/indexed_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15072 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/indexed_dataset/build_datasets.py
+-rwxr-xr-x   0 root         (0) root         (0)    23076 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/indexed_dataset/build_index_mappings.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/indexed_dataset/check_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/indexed_dataset/merge_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     8738 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/indexed_dataset/preprocess_data_args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/dataset/language_model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/language_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12850 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/language_model/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/dataset/mm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/mm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/mm/clip_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/dataset/seq2seq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/seq2seq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28134 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/seq2seq/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/dataset/superglue/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/superglue/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9434 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/superglue/control.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/superglue/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    64586 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/superglue/processor.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/superglue/properties.py
+-rw-r--r--   0 root         (0) root         (0)    64718 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/dataset/superglue/pvp.py
+-rwxrwxrwx   0 root         (0) root         (0)     8550 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/file_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/
+-rwxrwxrwx   0 root         (0) root         (0)      628 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/bert/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/bert/bert_tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    24023 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/bert/wordpiece.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/clip/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6261 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/clip/tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/cpm_1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/cpm_1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/cpm_1/cpm1_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/cpm_3/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/cpm_3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/cpm_3/cpm3_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/galactica/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/galactica/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/galactica/galactica_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/glm_10b_en/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_10b_en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12263 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_10b_en/glm_10b_en_bpe_tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    14814 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_10b_en/glm_10b_en_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/glm_large_ch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_large_ch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5250 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_large_ch/glm_large_ch.py
+-rw-r--r--   0 root         (0) root         (0)    10378 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_large_ch/glm_large_ch_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/glm_large_en/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_large_en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7982 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_large_en/glm_large_en_tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    13641 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/glm_large_en/wordpiece.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/llama/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/llama/tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.159077 flagai-1.7.2/flagai/data/tokenizer/opt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/opt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5003 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/opt/opt_en_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.163077 flagai-1.7.2/flagai/data/tokenizer/roberta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4930 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/roberta/roberta_tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.163077 flagai-1.7.2/flagai/data/tokenizer/t5/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/t5/t5_pegasus_tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    17572 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/t5/t5_tokenizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    18924 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.163077 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5450 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/base_tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)    12990 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/bpe_tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)    16106 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/diffusion_bert_tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)      242 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/properties.py
+-rwxr-xr-x   0 root         (0) root         (0)     2572 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/sp_tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)    35838 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)    13383 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/wp_tokenizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    16865 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/data/tokenizer/wp_tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)    13407 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/env_args.py
+-rwxr-xr-x   0 root         (0) root         (0)    45953 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/env_trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)    53951 2023-06-13 09:30:25.000000 flagai-1.7.2/flagai/env_trainer_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.163077 flagai-1.7.2/flagai/fp16/
+-rwxrwxrwx   0 root         (0) root         (0)      941 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/fp16/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    32292 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/fp16/fp16.py
+-rwxrwxrwx   0 root         (0) root         (0)     8015 2023-06-13 07:08:39.000000 flagai-1.7.2/flagai/fp16/fp16util.py
+-rwxrwxrwx   0 root         (0) root         (0)     8317 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/fp16/loss_scaler.py
+-rwxr-xr-x   0 root         (0) root         (0)     9467 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/launch.py
+-rwxr-xr-x   0 root         (0) root         (0)     3930 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/logger.py
+-rwxr-xr-x   0 root         (0) root         (0)     5303 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.163077 flagai-1.7.2/flagai/model/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      140 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/alm_model.py
+-rwxr-xr-x   0 root         (0) root         (0)     8737 2023-06-13 09:30:25.000000 flagai-1.7.2/flagai/model/aquila_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    12548 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/base_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    24995 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/bert_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.167077 flagai-1.7.2/flagai/model/blocks/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/blocks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2169 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/blocks/aquila_block.py
+-rwxrwxrwx   0 root         (0) root         (0)     4926 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/blocks/bert_block.py
+-rwxrwxrwx   0 root         (0) root         (0)    15383 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/blocks/cpm_block.py
+-rwxrwxrwx   0 root         (0) root         (0)     9222 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/blocks/glm_block.py
+-rwxrwxrwx   0 root         (0) root         (0)     2290 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/blocks/gpt2_block.py
+-rwxrwxrwx   0 root         (0) root         (0)     5307 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/blocks/t5_block.py
+-rwxrwxrwx   0 root         (0) root         (0)     1517 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    19137 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/cpm3_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    16321 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/cpm3_train_model.py
+-rwxrwxrwx   0 root         (0) root         (0)       75 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/cpm_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     5656 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/file_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     7998 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/galactica_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    40848 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/glm_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    15226 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/gpt2_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.167077 flagai-1.7.2/flagai/model/layers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7112 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/activations.py
+-rwxrwxrwx   0 root         (0) root         (0)    73399 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/attentions.py
+-rwxrwxrwx   0 root         (0) root         (0)    18699 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/attentions_bmt.py
+-rwxrwxrwx   0 root         (0) root         (0)     3063 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/crf.py
+-rwxrwxrwx   0 root         (0) root         (0)    21600 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/embeddings.py
+-rwxrwxrwx   0 root         (0) root         (0)     9666 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/embeddings_bmt.py
+-rwxrwxrwx   0 root         (0) root         (0)    27514 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/feedforward.py
+-rwxrwxrwx   0 root         (0) root         (0)    10505 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/feedforward_bmt.py
+-rwxrwxrwx   0 root         (0) root         (0)     4034 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/global_pointer.py
+-rwxrwxrwx   0 root         (0) root         (0)     4316 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/layer_norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2269 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/layer_norm_bmt.py
+-rwxrwxrwx   0 root         (0) root         (0)     2659 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/linear.py
+-rwxrwxrwx   0 root         (0) root         (0)     2959 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/layers/linear_bmt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.167077 flagai-1.7.2/flagai/model/mm/
+-rwxrwxrwx   0 root         (0) root         (0)    18852 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/AltCLIP.py
+-rwxrwxrwx   0 root         (0) root         (0)    81528 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/AltDiffusion.py
+-rwxrwxrwx   0 root         (0) root         (0)    85758 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/AltDiffusionM18.py
+-rwxrwxrwx   0 root         (0) root         (0)    25335 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/Sampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.167077 flagai-1.7.2/flagai/model/mm/Unets/
+-rw-r--r--   0 root         (0) root         (0)    35142 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/Unets/Unet.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/Unets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.167077 flagai-1.7.2/flagai/model/mm/attentions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/attentions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/attentions/attention.py
+-rwxrwxrwx   0 root         (0) root         (0)     8609 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/autoencoder_m18.py
+-rwxrwxrwx   0 root         (0) root         (0)    18905 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/autoencoders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.167077 flagai-1.7.2/flagai/model/mm/clip_guohua/
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/clip_guohua/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14839 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/clip_guohua/bert_tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/clip_guohua/clip.py
+-rw-r--r--   0 root         (0) root         (0)     3905 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/clip_guohua/configuration_bert.py
+-rw-r--r--   0 root         (0) root         (0)    18569 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/clip_guohua/model.py
+-rw-r--r--   0 root         (0) root         (0)    20144 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/clip_guohua/modeling_bert.py
+-rwxrwxrwx   0 root         (0) root         (0)    12489 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/clip_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/mm/dpm_solver/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/dpm_solver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65969 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/dpm_solver/dpm_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/dpm_solver/sampler.py
+-rwxrwxrwx   0 root         (0) root         (0)    24330 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/eva_clip_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/mm/lm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/lm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/lm/clip_guohua.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/lm/dcn_clip.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/lm/en_clip.py
+-rw-r--r--   0 root         (0) root         (0)    20168 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/lm/x_transformer.py
+-rwxrwxrwx   0 root         (0) root         (0)    38506 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/model.py
+-rwxrwxrwx   0 root         (0) root         (0)    67851 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modeling_altclip.py
+-rwxrwxrwx   0 root         (0) root         (0)     5632 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modeling_berts.py
+-rwxrwxrwx   0 root         (0) root         (0)     6277 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modeling_berts_m18.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/mm/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11904 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/attention.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34396 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/model.py
+-rw-r--r--   0 root         (0) root         (0)    35811 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 root         (0) root         (0)     9881 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/mm/modules/distributions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/distributions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/distributions/distributions.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/modules/ema.py
+-rwxrwxrwx   0 root         (0) root         (0)    21130 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/mm/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     8308 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/opt_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/predictor/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/predictor/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3106 2023-06-13 09:31:50.000000 flagai-1.7.2/flagai/model/predictor/aquila.py
+-rwxrwxrwx   0 root         (0) root         (0)     2614 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/predictor/gpt.py
+-rwxrwxrwx   0 root         (0) root         (0)    23314 2023-06-13 07:35:39.000000 flagai-1.7.2/flagai/model/predictor/predictor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5315 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/predictor/simctg.py
+-rwxrwxrwx   0 root         (0) root         (0)    91302 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/predictor/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2561 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/prompt.py
+-rwxrwxrwx   0 root         (0) root         (0)    57714 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/t5_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/tools/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 07:08:39.000000 flagai-1.7.2/flagai/model/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/tools/lora/
+-rwxr-xr-x   0 root         (0) root         (0)     1204 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      720 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/import_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     3304 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/mapping.py
+-rwxr-xr-x   0 root         (0) root         (0)     4343 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/mappings.py
+-rwxr-xr-x   0 root         (0) root         (0)    51884 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/peft_model.py
+-rwxr-xr-x   0 root         (0) root         (0)     1028 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/prepare_lora.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/tools/lora/tuners/
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/tuners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24927 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/tuners/lora.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/tools/lora/utils/
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/utils/other.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/tools/lora/utils/save_and_load.py
+-rwxrwxrwx   0 root         (0) root         (0)     2370 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.171077 flagai-1.7.2/flagai/model/vision/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2857 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.179077 flagai-1.7.2/flagai/model/vision/layers/
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/activations.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/activations_jit.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/activations_me.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/adaptive_avgmax_pool.py
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/attention_pool2d.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/blur_pool.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/bottleneck_attn.py
+-rw-r--r--   0 root         (0) root         (0)     4426 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/cbam.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/classifier.py
+-rw-r--r--   0 root         (0) root         (0)     5199 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/cond_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/config.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/conv2d_same.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/conv_bn_act.py
+-rw-r--r--   0 root         (0) root         (0)     5104 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/create_act.py
+-rw-r--r--   0 root         (0) root         (0)     3526 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/create_attn.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/create_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     3562 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/create_norm_act.py
+-rw-r--r--   0 root         (0) root         (0)     6786 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/drop.py
+-rw-r--r--   0 root         (0) root         (0)     6386 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/eca.py
+-rw-r--r--   0 root         (0) root         (0)    13792 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/evo_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/filter_response_norm.py
+-rw-r--r--   0 root         (0) root         (0)     3824 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/gather_excite.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/global_context.py
+-rw-r--r--   0 root         (0) root         (0)    10662 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/halo_attn.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/inplace_abn.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/lambda_layer.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/linear.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/median_pool.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/mixed_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     7008 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/ml_decoder.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/mlp.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/non_local_attn.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/norm.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/norm_act.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/padding.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/patch_embed.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/pool2d_same.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/pos_embed.py
+-rw-r--r--   0 root         (0) root         (0)     5387 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/selective_kernel.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/separable_conv.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/space_to_depth.py
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/split_attn.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/split_batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/squeeze_excite.py
+-rw-r--r--   0 root         (0) root         (0)     5887 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/std_conv.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/test_time_pool.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/trace_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3265 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/layers/weight_init.py
+-rwxrwxrwx   0 root         (0) root         (0)    28804 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/swinv1.py
+-rwxrwxrwx   0 root         (0) root         (0)    29099 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/swinv2.py
+-rwxrwxrwx   0 root         (0) root         (0)    23433 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/model/vision/vit.py
+-rwxr-xr-x   0 root         (0) root         (0)    16329 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mp_tools.py
+-rwxr-xr-x   0 root         (0) root         (0)     7391 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mp_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.179077 flagai-1.7.2/flagai/mpu/
+-rwxrwxrwx   0 root         (0) root         (0)     1637 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4952 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/cross_entropy.py
+-rwxrwxrwx   0 root         (0) root         (0)     4143 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     1509 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/func_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3227 2023-06-13 07:09:14.000000 flagai-1.7.2/flagai/mpu/grads.py
+-rwxrwxrwx   0 root         (0) root         (0)     4973 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/initialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     2287 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/local_attention_function.py
+-rwxrwxrwx   0 root         (0) root         (0)     4254 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/mappings.py
+-rwxrwxrwx   0 root         (0) root         (0)    14979 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/random.py
+-rwxrwxrwx   0 root         (0) root         (0)     2899 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/mpu/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     5772 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/optimizers.py
+-rwxr-xr-x   0 root         (0) root         (0)     6043 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/schedulers.py
+-rwxr-xr-x   0 root         (0) root         (0)     5616 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/test_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    50816 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)    60172 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/trainer_v1.py
+-rwxr-xr-x   0 root         (0) root         (0)    12428 2023-06-13 05:25:15.000000 flagai-1.7.2/flagai/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.155077 flagai-1.7.2/flagai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20437 2023-06-13 09:35:24.000000 flagai-1.7.2/flagai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10086 2023-06-13 09:35:24.000000 flagai-1.7.2/flagai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 09:35:24.000000 flagai-1.7.2/flagai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      342 2023-06-13 09:35:24.000000 flagai-1.7.2/flagai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 09:35:24.000000 flagai-1.7.2/flagai.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-06-13 09:35:24.179077 flagai-1.7.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1310 2023-06-13 09:35:20.000000 flagai-1.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:35:24.179077 flagai-1.7.2/tests/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3645 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/bak_test_superglue.py
+-rwxr-xr-x   0 root         (0) root         (0)     1538 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/bak_test_t5_ch.py
+-rwxr-xr-x   0 root         (0) root         (0)     5251 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/test_autoloader.py
+-rwxr-xr-x   0 root         (0) root         (0)     2500 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/test_bert.py
+-rwxr-xr-x   0 root         (0) root         (0)     1399 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/test_glm_large_ch.py
+-rwxr-xr-x   0 root         (0) root         (0)     2755 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/test_glm_seq2seq.py
+-rwxr-xr-x   0 root         (0) root         (0)     1009 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/test_gpt2_ch.py
+-rwxr-xr-x   0 root         (0) root         (0)    11246 2023-06-13 05:25:15.000000 flagai-1.7.2/tests/test_tokenizer.py
```

### Comparing `flagai-1.7.1/LICENSE` & `flagai-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/PKG-INFO` & `flagai-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: flagai
-Version: 1.7.1
+Version: 1.7.2
 Summary: FlagAI aims to help researchers and developers to freely train and test large-scale models for NLP/CV/VL tasks.
 Home-page: https://github.com/FlagAI-Open/FlagAI
 Author: FlagAI-Open
 Author-email: open@baai.ac.cn
 License: Apache 2.0
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![FlagAI](logo.png)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6052/badge)](https://bestpractices.coreinfrastructure.org/projects/6052)
 [![Python application](https://github.com/FlagAI-Open/FlagAI/actions/workflows/python-app.yml/badge.svg)](https://github.com/FlagAI-Open/FlagAI/actions/workflows/python-app.yml)
@@ -129,15 +130,15 @@
 
 
 ## Quick Start
 We provide many models which are trained to perform different tasks. You can load these models by AutoLoader to make prediction. See more in `FlagAI/quickstart`.
 
 ### Requirements and Installation
 * Python version >= 3.8
-* PyTorch version >= 1.8.0
+* PyTorch version >= 1.12.0
 * [Optional] For training/testing models on GPUs, you'll also need to install CUDA and NCCL
 
 - To install FlagAI with pip:
 ```shell
 pip install -U flagai
 ```
 
@@ -150,28 +151,38 @@
 
 - [Optional] For faster training, install NVIDIA's [apex](https://github.com/NVIDIA/apex)
 ```
 git clone https://github.com/NVIDIA/apex
 cd apex
 pip install -v --disable-pip-version-check --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" ./
 ```
-- [Optional] For ZeRO optimizers, install [DEEPSPEED](https://github.com/microsoft/DeepSpeed)
+- [Optional] For ZeRO optimizers, install [DEEPSPEED](https://github.com/microsoft/DeepSpeed) (>= 0.7.7)
 ```
 git clone https://github.com/microsoft/DeepSpeed
 cd DeepSpeed
 DS_BUILD_CPU_ADAM=1 DS_BUILD_AIO=1 DS_BUILD_UTILS=1 pip install -e .
 ds_report # check the deespeed status
 ```
-- [Optional] For BMTrain training, install [BMTrain](https://github.com/OpenBMB/BMTrain)
+- [Optional] For BMTrain training, install [BMTrain](https://github.com/OpenBMB/BMTrain) (>= 0.2.2)
 ```
 git clone https://github.com/OpenBMB/BMTrain
 cd BMTrain
 python setup.py install
 ```
-- [Tips] For single-node docker environments, we need to set up ports for your ssh. e.g., root@127.0.0.1 with port 7110
+- [Optional] For BMInf low-resource inference, install [BMInf](https://github.com/OpenBMB/BMInf)
+```
+pip install bminf
+
+```
+- [Optional] For Flash Attention, install [Flash-attention](https://github.com/HazyResearch/flash-attention) (>=1.0.2)
+```
+pip install flash-attn
+```
+
+- [Tips] For single-node docker environments, we need to set up ports for your ssh. e.g., root@127.0.0.1 with port 711
 ```
 >>> vim ~/.ssh/config
 Host 127.0.0.1
     Hostname 127.0.0.1
     Port 7110
     User root
 ```
@@ -325,7 +336,9 @@
 
 ### &#8627; Star History
 <div align="center">
 
 ![Star History Chart](https://api.star-history.com/svg?repos=FlagAI-Open/FlagAI&type=Date)]
 
 </div>
+
+
```

### Comparing `flagai-1.7.1/README.md` & `flagai-1.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 
 ## Quick Start
 We provide many models which are trained to perform different tasks. You can load these models by AutoLoader to make prediction. See more in `FlagAI/quickstart`.
 
 ### Requirements and Installation
 * Python version >= 3.8
-* PyTorch version >= 1.8.0
+* PyTorch version >= 1.12.0
 * [Optional] For training/testing models on GPUs, you'll also need to install CUDA and NCCL
 
 - To install FlagAI with pip:
 ```shell
 pip install -U flagai
 ```
 
@@ -138,28 +138,38 @@
 
 - [Optional] For faster training, install NVIDIA's [apex](https://github.com/NVIDIA/apex)
 ```
 git clone https://github.com/NVIDIA/apex
 cd apex
 pip install -v --disable-pip-version-check --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" ./
 ```
-- [Optional] For ZeRO optimizers, install [DEEPSPEED](https://github.com/microsoft/DeepSpeed)
+- [Optional] For ZeRO optimizers, install [DEEPSPEED](https://github.com/microsoft/DeepSpeed) (>= 0.7.7)
 ```
 git clone https://github.com/microsoft/DeepSpeed
 cd DeepSpeed
 DS_BUILD_CPU_ADAM=1 DS_BUILD_AIO=1 DS_BUILD_UTILS=1 pip install -e .
 ds_report # check the deespeed status
 ```
-- [Optional] For BMTrain training, install [BMTrain](https://github.com/OpenBMB/BMTrain)
+- [Optional] For BMTrain training, install [BMTrain](https://github.com/OpenBMB/BMTrain) (>= 0.2.2)
 ```
 git clone https://github.com/OpenBMB/BMTrain
 cd BMTrain
 python setup.py install
 ```
-- [Tips] For single-node docker environments, we need to set up ports for your ssh. e.g., root@127.0.0.1 with port 7110
+- [Optional] For BMInf low-resource inference, install [BMInf](https://github.com/OpenBMB/BMInf)
+```
+pip install bminf
+
+```
+- [Optional] For Flash Attention, install [Flash-attention](https://github.com/HazyResearch/flash-attention) (>=1.0.2)
+```
+pip install flash-attn
+```
+
+- [Tips] For single-node docker environments, we need to set up ports for your ssh. e.g., root@127.0.0.1 with port 711
 ```
 >>> vim ~/.ssh/config
 Host 127.0.0.1
     Hostname 127.0.0.1
     Port 7110
     User root
 ```
```

### Comparing `flagai-1.7.1/flagai/auto_model/auto_loader.py` & `flagai-1.7.2/flagai/auto_model/auto_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,16 +216,14 @@
         self.model = getattr(LazyImport(self.model_name[0]),
                              self.model_name[1]).from_pretrain(
             download_path=model_dir,
             model_name=model_name_,
             only_download_config=only_download_config,
             device=device,
             **kwargs)
-        if kwargs.get("use_fp16", None):
-            self.model.half()
         
         if model_type == "nlp":
             if brief_model_name in ["galactica",]:
                 self.tokenizer = getattr(LazyImport(MODEL_DICT[model_name][4]),
                                                     MODEL_DICT[model_name][5])(download_path)
             else :
                 tokenizer_class = getattr(LazyImport("flagai.data.tokenizer"),
```

### Comparing `flagai-1.7.1/flagai/data/collate_utils.py` & `flagai-1.7.2/flagai/data/collate_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/block/blocklm_utils.py` & `flagai-1.7.2/flagai/data/dataset/block/blocklm_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/block/corpora.py` & `flagai-1.7.2/flagai/data/dataset/block/corpora.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/block/data_utils.py` & `flagai-1.7.2/flagai/data/dataset/block/data_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/block/dataset.py` & `flagai-1.7.2/flagai/data/dataset/block/dataset.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/block/lazy_loader.py` & `flagai-1.7.2/flagai/data/dataset/block/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/cpm3_data/dataset.py` & `flagai-1.7.2/flagai/data/dataset/cpm3_data/dataset.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/cpm3_data/distributed_indexed.py` & `flagai-1.7.2/flagai/data/dataset/cpm3_data/distributed_indexed.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/cpm3_data/indexed.py` & `flagai-1.7.2/flagai/data/dataset/cpm3_data/indexed.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/data_collator/collate_fn.py` & `flagai-1.7.2/flagai/data/dataset/data_collator/collate_fn.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/data_utils.py` & `flagai-1.7.2/flagai/data/dataset/data_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/indexed_dataset/build_datasets.py` & `flagai-1.7.2/flagai/data/dataset/indexed_dataset/build_datasets.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/indexed_dataset/build_index_mappings.py` & `flagai-1.7.2/flagai/data/dataset/indexed_dataset/build_index_mappings.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/indexed_dataset/check_datasets.py` & `flagai-1.7.2/flagai/data/dataset/indexed_dataset/check_datasets.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/indexed_dataset/merge_datasets.py` & `flagai-1.7.2/flagai/data/dataset/indexed_dataset/merge_datasets.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/indexed_dataset/preprocess_data_args.py` & `flagai-1.7.2/flagai/data/dataset/indexed_dataset/preprocess_data_args.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/language_model/dataset.py` & `flagai-1.7.2/flagai/data/dataset/language_model/dataset.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/mm/clip_dataset.py` & `flagai-1.7.2/flagai/data/dataset/mm/clip_dataset.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/seq2seq/dataset.py` & `flagai-1.7.2/flagai/data/dataset/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/superglue/control.py` & `flagai-1.7.2/flagai/data/dataset/superglue/control.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/superglue/dataset.py` & `flagai-1.7.2/flagai/data/dataset/superglue/dataset.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/superglue/processor.py` & `flagai-1.7.2/flagai/data/dataset/superglue/processor.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/superglue/properties.py` & `flagai-1.7.2/flagai/data/dataset/superglue/properties.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/dataset/superglue/pvp.py` & `flagai-1.7.2/flagai/data/dataset/superglue/pvp.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/file_utils.py` & `flagai-1.7.2/flagai/data/file_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/__init__.py` & `flagai-1.7.2/flagai/data/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/bert/bert_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/bert/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/bert/wordpiece.py` & `flagai-1.7.2/flagai/data/tokenizer/bert/wordpiece.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/clip/tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/cpm_1/cpm1_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/cpm_1/cpm1_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/cpm_3/cpm3_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/cpm_3/cpm3_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/galactica/galactica_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/galactica/galactica_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/glm_10b_en/glm_10b_en_bpe_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/glm_10b_en/glm_10b_en_bpe_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/glm_10b_en/glm_10b_en_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/glm_10b_en/glm_10b_en_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/glm_large_ch/glm_large_ch.py` & `flagai-1.7.2/flagai/data/tokenizer/glm_large_ch/glm_large_ch.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/glm_large_ch/glm_large_ch_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/glm_large_ch/glm_large_ch_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/glm_large_en/glm_large_en_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/glm_large_en/glm_large_en_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/glm_large_en/wordpiece.py` & `flagai-1.7.2/flagai/data/tokenizer/glm_large_en/wordpiece.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/llama/tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/llama/tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/opt/opt_en_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/opt/opt_en_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/roberta/roberta_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/roberta/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/t5/t5_pegasus_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/t5/t5_pegasus_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/t5/t5_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/t5/t5_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/base_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/bpe_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/bpe_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/diffusion_bert_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/diffusion_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/sp_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/uni_tokenizer/wp_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/uni_tokenizer/wp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/data/tokenizer/wp_tokenizer.py` & `flagai-1.7.2/flagai/data/tokenizer/wp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/env_args.py` & `flagai-1.7.2/flagai/env_args.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/env_trainer.py` & `flagai-1.7.2/flagai/env_trainer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/env_trainer_v1.py` & `flagai-1.7.2/flagai/env_trainer_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,15 +567,15 @@
                                                            self.optimizer,
                                                            lr_scheduler,
                                                            single_step=True)
                     dist.barrier()
 
                 if lm_loss is not None:
                     if not isinstance(lm_loss, float):
-                        total_lm_loss += lm_loss.data.detach().float()
+                        total_lm_loss += lm_loss.data.detach().item()
                     else:
                         total_lm_loss += lm_loss
 
                 if 'bmtrain' in self.env_type and cached is not None and 'grad_norm' in cached:
                     total_grad_norm += cached['grad_norm']
 
                 # Logging.
```

### Comparing `flagai-1.7.1/flagai/fp16/__init__.py` & `flagai-1.7.2/flagai/fp16/__init__.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/fp16/fp16.py` & `flagai-1.7.2/flagai/fp16/fp16.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/fp16/fp16util.py` & `flagai-1.7.2/flagai/fp16/fp16util.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     def forward(self, *inputs):
         inputs = tuple(t.half() for t in inputs)
         return self.network(*inputs)
 
 
 def backwards_debug_hook(grad):
     raise RuntimeError(
-        "master_params recieved a gradient in the backward pass!")
+        "master_params received a gradient in the backward pass!")
 
 
 def prep_param_lists(model, flat_master=False):
     """
     Creates a list of FP32 master parameters for a given model, as in
     `Training Neural Networks with Mixed Precision:  Real Examples`_.
```

### Comparing `flagai-1.7.1/flagai/fp16/loss_scaler.py` & `flagai-1.7.2/flagai/fp16/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/launch.py` & `flagai-1.7.2/flagai/launch.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/logger.py` & `flagai-1.7.2/flagai/logger.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/metrics.py` & `flagai-1.7.2/flagai/metrics.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/base_model.py` & `flagai-1.7.2/flagai/model/base_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/bert_model.py` & `flagai-1.7.2/flagai/model/bert_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/blocks/aquila_block.py` & `flagai-1.7.2/flagai/model/blocks/aquila_block.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/blocks/bert_block.py` & `flagai-1.7.2/flagai/model/blocks/bert_block.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/blocks/cpm_block.py` & `flagai-1.7.2/flagai/model/blocks/cpm_block.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/blocks/glm_block.py` & `flagai-1.7.2/flagai/model/blocks/glm_block.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/blocks/gpt2_block.py` & `flagai-1.7.2/flagai/model/blocks/gpt2_block.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/blocks/t5_block.py` & `flagai-1.7.2/flagai/model/blocks/t5_block.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/config.py` & `flagai-1.7.2/flagai/model/config.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/cpm3_model.py` & `flagai-1.7.2/flagai/model/cpm3_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/cpm3_train_model.py` & `flagai-1.7.2/flagai/model/cpm3_train_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/file_utils.py` & `flagai-1.7.2/flagai/model/file_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/galactica_model.py` & `flagai-1.7.2/flagai/model/galactica_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/glm_model.py` & `flagai-1.7.2/flagai/model/glm_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/gpt2_model.py` & `flagai-1.7.2/flagai/model/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/activations.py` & `flagai-1.7.2/flagai/model/layers/activations.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/attentions.py` & `flagai-1.7.2/flagai/model/layers/attentions.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/attentions_bmt.py` & `flagai-1.7.2/flagai/model/layers/attentions_bmt.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/crf.py` & `flagai-1.7.2/flagai/model/layers/crf.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/embeddings.py` & `flagai-1.7.2/flagai/model/layers/embeddings.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/embeddings_bmt.py` & `flagai-1.7.2/flagai/model/layers/embeddings_bmt.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/feedforward.py` & `flagai-1.7.2/flagai/model/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/feedforward_bmt.py` & `flagai-1.7.2/flagai/model/layers/feedforward_bmt.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/global_pointer.py` & `flagai-1.7.2/flagai/model/layers/global_pointer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/layer_norm.py` & `flagai-1.7.2/flagai/model/layers/layer_norm.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/layer_norm_bmt.py` & `flagai-1.7.2/flagai/model/layers/layer_norm_bmt.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/linear.py` & `flagai-1.7.2/flagai/model/layers/linear.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/layers/linear_bmt.py` & `flagai-1.7.2/flagai/model/layers/linear_bmt.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/AltCLIP.py` & `flagai-1.7.2/flagai/model/mm/AltCLIP.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/AltDiffusion.py` & `flagai-1.7.2/flagai/model/mm/AltDiffusion.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/AltDiffusionM18.py` & `flagai-1.7.2/flagai/model/mm/AltDiffusionM18.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/Sampler.py` & `flagai-1.7.2/flagai/model/mm/Sampler.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/Unets/Unet.py` & `flagai-1.7.2/flagai/model/mm/Unets/Unet.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/attentions/attention.py` & `flagai-1.7.2/flagai/model/mm/attentions/attention.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/autoencoder_m18.py` & `flagai-1.7.2/flagai/model/mm/autoencoder_m18.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/autoencoders.py` & `flagai-1.7.2/flagai/model/mm/autoencoders.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/clip_guohua/bert_tokenizer.py` & `flagai-1.7.2/flagai/model/mm/clip_guohua/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/clip_guohua/clip.py` & `flagai-1.7.2/flagai/model/mm/clip_guohua/clip.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/clip_guohua/configuration_bert.py` & `flagai-1.7.2/flagai/model/mm/clip_guohua/configuration_bert.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/clip_guohua/model.py` & `flagai-1.7.2/flagai/model/mm/clip_guohua/model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/clip_guohua/modeling_bert.py` & `flagai-1.7.2/flagai/model/mm/clip_guohua/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/clip_model.py` & `flagai-1.7.2/flagai/model/mm/clip_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/dpm_solver/dpm_solver.py` & `flagai-1.7.2/flagai/model/mm/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/dpm_solver/sampler.py` & `flagai-1.7.2/flagai/model/mm/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/eva_clip_model.py` & `flagai-1.7.2/flagai/model/mm/eva_clip_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/lm/clip_guohua.py` & `flagai-1.7.2/flagai/model/mm/lm/clip_guohua.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/lm/dcn_clip.py` & `flagai-1.7.2/flagai/model/mm/lm/dcn_clip.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/lm/en_clip.py` & `flagai-1.7.2/flagai/model/mm/lm/en_clip.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/lm/x_transformer.py` & `flagai-1.7.2/flagai/model/mm/lm/x_transformer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/model.py` & `flagai-1.7.2/flagai/model/mm/model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modeling_altclip.py` & `flagai-1.7.2/flagai/model/mm/modeling_altclip.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modeling_berts.py` & `flagai-1.7.2/flagai/model/mm/modeling_berts.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modeling_berts_m18.py` & `flagai-1.7.2/flagai/model/mm/modeling_berts_m18.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modules/attention.py` & `flagai-1.7.2/flagai/model/mm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/model.py` & `flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/openaimodel.py` & `flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modules/diffusionmodules/util.py` & `flagai-1.7.2/flagai/model/mm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modules/distributions/distributions.py` & `flagai-1.7.2/flagai/model/mm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/modules/ema.py` & `flagai-1.7.2/flagai/model/mm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/mm/utils.py` & `flagai-1.7.2/flagai/model/mm/utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/opt_model.py` & `flagai-1.7.2/flagai/model/opt_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/predictor/gpt.py` & `flagai-1.7.2/flagai/model/predictor/gpt.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/predictor/predictor.py` & `flagai-1.7.2/flagai/model/predictor/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
             return bert_random_sample(self.model, self.tokenizer, text,
                                       input_max_length, out_max_length, top_k,
                                       top_p, repetition_penalty, temperature,
                                       device)
         elif "aquila" in self.class_name.lower():
             return aquila_generate(self.tokenizer, self.model,
                                   [text], out_max_length,
-                                  temperature, top_p, prompts_tokens=prompts_tokens)
+                                  temperature, top_k, top_p, prompts_tokens=prompts_tokens)
 
         else:
             print("Unsupported decoding mode")
             import os
             os._exit(0)
```

### Comparing `flagai-1.7.1/flagai/model/predictor/simctg.py` & `flagai-1.7.2/flagai/model/predictor/simctg.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/predictor/utils.py` & `flagai-1.7.2/flagai/model/predictor/utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/prompt.py` & `flagai-1.7.2/flagai/model/prompt.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/t5_model.py` & `flagai-1.7.2/flagai/model/t5_model.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/utils.py` & `flagai-1.7.2/flagai/model/utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/helpers.py` & `flagai-1.7.2/flagai/model/vision/helpers.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/__init__.py` & `flagai-1.7.2/flagai/model/vision/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/activations.py` & `flagai-1.7.2/flagai/model/vision/layers/activations.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/activations_jit.py` & `flagai-1.7.2/flagai/model/vision/layers/activations_jit.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/activations_me.py` & `flagai-1.7.2/flagai/model/vision/layers/activations_me.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/adaptive_avgmax_pool.py` & `flagai-1.7.2/flagai/model/vision/layers/adaptive_avgmax_pool.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/attention_pool2d.py` & `flagai-1.7.2/flagai/model/vision/layers/attention_pool2d.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/blur_pool.py` & `flagai-1.7.2/flagai/model/vision/layers/blur_pool.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/bottleneck_attn.py` & `flagai-1.7.2/flagai/model/vision/layers/bottleneck_attn.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/cbam.py` & `flagai-1.7.2/flagai/model/vision/layers/cbam.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/classifier.py` & `flagai-1.7.2/flagai/model/vision/layers/classifier.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/cond_conv2d.py` & `flagai-1.7.2/flagai/model/vision/layers/cond_conv2d.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/config.py` & `flagai-1.7.2/flagai/model/vision/layers/config.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/conv2d_same.py` & `flagai-1.7.2/flagai/model/vision/layers/conv2d_same.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/conv_bn_act.py` & `flagai-1.7.2/flagai/model/vision/layers/conv_bn_act.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/create_act.py` & `flagai-1.7.2/flagai/model/vision/layers/create_act.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/create_attn.py` & `flagai-1.7.2/flagai/model/vision/layers/create_attn.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/create_conv2d.py` & `flagai-1.7.2/flagai/model/vision/layers/create_conv2d.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/create_norm_act.py` & `flagai-1.7.2/flagai/model/vision/layers/create_norm_act.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/drop.py` & `flagai-1.7.2/flagai/model/vision/layers/drop.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/eca.py` & `flagai-1.7.2/flagai/model/vision/layers/eca.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/evo_norm.py` & `flagai-1.7.2/flagai/model/vision/layers/evo_norm.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/filter_response_norm.py` & `flagai-1.7.2/flagai/model/vision/layers/filter_response_norm.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/gather_excite.py` & `flagai-1.7.2/flagai/model/vision/layers/gather_excite.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/global_context.py` & `flagai-1.7.2/flagai/model/vision/layers/global_context.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/halo_attn.py` & `flagai-1.7.2/flagai/model/vision/layers/halo_attn.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/helpers.py` & `flagai-1.7.2/flagai/model/vision/layers/helpers.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/inplace_abn.py` & `flagai-1.7.2/flagai/model/vision/layers/inplace_abn.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/lambda_layer.py` & `flagai-1.7.2/flagai/model/vision/layers/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/linear.py` & `flagai-1.7.2/flagai/model/vision/layers/linear.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/median_pool.py` & `flagai-1.7.2/flagai/model/vision/layers/median_pool.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/mixed_conv2d.py` & `flagai-1.7.2/flagai/model/vision/layers/mixed_conv2d.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/ml_decoder.py` & `flagai-1.7.2/flagai/model/vision/layers/ml_decoder.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/mlp.py` & `flagai-1.7.2/flagai/model/vision/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/non_local_attn.py` & `flagai-1.7.2/flagai/model/vision/layers/non_local_attn.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/norm.py` & `flagai-1.7.2/flagai/model/vision/layers/norm.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/norm_act.py` & `flagai-1.7.2/flagai/model/vision/layers/norm_act.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/padding.py` & `flagai-1.7.2/flagai/model/vision/layers/padding.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/patch_embed.py` & `flagai-1.7.2/flagai/model/vision/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/pool2d_same.py` & `flagai-1.7.2/flagai/model/vision/layers/pool2d_same.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/pos_embed.py` & `flagai-1.7.2/flagai/model/vision/layers/pos_embed.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/selective_kernel.py` & `flagai-1.7.2/flagai/model/vision/layers/selective_kernel.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/separable_conv.py` & `flagai-1.7.2/flagai/model/vision/layers/separable_conv.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/space_to_depth.py` & `flagai-1.7.2/flagai/model/vision/layers/space_to_depth.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/split_attn.py` & `flagai-1.7.2/flagai/model/vision/layers/split_attn.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/split_batchnorm.py` & `flagai-1.7.2/flagai/model/vision/layers/split_batchnorm.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/squeeze_excite.py` & `flagai-1.7.2/flagai/model/vision/layers/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/std_conv.py` & `flagai-1.7.2/flagai/model/vision/layers/std_conv.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/test_time_pool.py` & `flagai-1.7.2/flagai/model/vision/layers/test_time_pool.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/layers/weight_init.py` & `flagai-1.7.2/flagai/model/vision/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/swinv1.py` & `flagai-1.7.2/flagai/model/vision/swinv1.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/swinv2.py` & `flagai-1.7.2/flagai/model/vision/swinv2.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/model/vision/vit.py` & `flagai-1.7.2/flagai/model/vision/vit.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mp_tools.py` & `flagai-1.7.2/flagai/mp_tools.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mp_utils.py` & `flagai-1.7.2/flagai/mp_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/__init__.py` & `flagai-1.7.2/flagai/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/cross_entropy.py` & `flagai-1.7.2/flagai/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/data.py` & `flagai-1.7.2/flagai/mpu/data.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/func_utils.py` & `flagai-1.7.2/flagai/mpu/func_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/grads.py` & `flagai-1.7.2/flagai/mpu/grads.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Parts of the code here are adapted from PyTorch
 # repo: https://github.com/pytorch/pytorch
 
 import torch
-from torch._six import inf
+import sys
+if torch.__version__ >= "2" and sys.platform != "win32":
+    from torch import inf
+else:
+    from torch._six import inf
 
 from .initialize import get_model_parallel_group
 from .initialize import get_model_parallel_rank
 
 
 def clip_grad_norm(parameters, max_norm, norm_type=2):
     """Clips gradient norm of an iterable of parameters.
```

### Comparing `flagai-1.7.1/flagai/mpu/initialize.py` & `flagai-1.7.2/flagai/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/local_attention_function.py` & `flagai-1.7.2/flagai/mpu/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/mappings.py` & `flagai-1.7.2/flagai/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/random.py` & `flagai-1.7.2/flagai/mpu/random.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/mpu/utils.py` & `flagai-1.7.2/flagai/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/optimizers.py` & `flagai-1.7.2/flagai/optimizers.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/schedulers.py` & `flagai-1.7.2/flagai/schedulers.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/test_utils.py` & `flagai-1.7.2/flagai/test_utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/trainer.py` & `flagai-1.7.2/flagai/trainer.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/trainer_v1.py` & `flagai-1.7.2/flagai/trainer_v1.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai/utils.py` & `flagai-1.7.2/flagai/utils.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/flagai.egg-info/PKG-INFO` & `flagai-1.7.2/flagai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: flagai
-Version: 1.7.1
+Version: 1.7.2
 Summary: FlagAI aims to help researchers and developers to freely train and test large-scale models for NLP/CV/VL tasks.
 Home-page: https://github.com/FlagAI-Open/FlagAI
 Author: FlagAI-Open
 Author-email: open@baai.ac.cn
 License: Apache 2.0
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![FlagAI](logo.png)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6052/badge)](https://bestpractices.coreinfrastructure.org/projects/6052)
 [![Python application](https://github.com/FlagAI-Open/FlagAI/actions/workflows/python-app.yml/badge.svg)](https://github.com/FlagAI-Open/FlagAI/actions/workflows/python-app.yml)
@@ -129,15 +130,15 @@
 
 
 ## Quick Start
 We provide many models which are trained to perform different tasks. You can load these models by AutoLoader to make prediction. See more in `FlagAI/quickstart`.
 
 ### Requirements and Installation
 * Python version >= 3.8
-* PyTorch version >= 1.8.0
+* PyTorch version >= 1.12.0
 * [Optional] For training/testing models on GPUs, you'll also need to install CUDA and NCCL
 
 - To install FlagAI with pip:
 ```shell
 pip install -U flagai
 ```
 
@@ -150,28 +151,38 @@
 
 - [Optional] For faster training, install NVIDIA's [apex](https://github.com/NVIDIA/apex)
 ```
 git clone https://github.com/NVIDIA/apex
 cd apex
 pip install -v --disable-pip-version-check --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" ./
 ```
-- [Optional] For ZeRO optimizers, install [DEEPSPEED](https://github.com/microsoft/DeepSpeed)
+- [Optional] For ZeRO optimizers, install [DEEPSPEED](https://github.com/microsoft/DeepSpeed) (>= 0.7.7)
 ```
 git clone https://github.com/microsoft/DeepSpeed
 cd DeepSpeed
 DS_BUILD_CPU_ADAM=1 DS_BUILD_AIO=1 DS_BUILD_UTILS=1 pip install -e .
 ds_report # check the deespeed status
 ```
-- [Optional] For BMTrain training, install [BMTrain](https://github.com/OpenBMB/BMTrain)
+- [Optional] For BMTrain training, install [BMTrain](https://github.com/OpenBMB/BMTrain) (>= 0.2.2)
 ```
 git clone https://github.com/OpenBMB/BMTrain
 cd BMTrain
 python setup.py install
 ```
-- [Tips] For single-node docker environments, we need to set up ports for your ssh. e.g., root@127.0.0.1 with port 7110
+- [Optional] For BMInf low-resource inference, install [BMInf](https://github.com/OpenBMB/BMInf)
+```
+pip install bminf
+
+```
+- [Optional] For Flash Attention, install [Flash-attention](https://github.com/HazyResearch/flash-attention) (>=1.0.2)
+```
+pip install flash-attn
+```
+
+- [Tips] For single-node docker environments, we need to set up ports for your ssh. e.g., root@127.0.0.1 with port 711
 ```
 >>> vim ~/.ssh/config
 Host 127.0.0.1
     Hostname 127.0.0.1
     Port 7110
     User root
 ```
@@ -325,7 +336,9 @@
 
 ### &#8627; Star History
 <div align="center">
 
 ![Star History Chart](https://api.star-history.com/svg?repos=FlagAI-Open/FlagAI&type=Date)]
 
 </div>
+
+
```

### Comparing `flagai-1.7.1/flagai.egg-info/SOURCES.txt` & `flagai-1.7.2/flagai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -184,14 +184,27 @@
 flagai/model/mm/modules/distributions/distributions.py
 flagai/model/predictor/__init__.py
 flagai/model/predictor/aquila.py
 flagai/model/predictor/gpt.py
 flagai/model/predictor/predictor.py
 flagai/model/predictor/simctg.py
 flagai/model/predictor/utils.py
+flagai/model/tools/__init__.py
+flagai/model/tools/lora/__init__.py
+flagai/model/tools/lora/import_utils.py
+flagai/model/tools/lora/mapping.py
+flagai/model/tools/lora/mappings.py
+flagai/model/tools/lora/peft_model.py
+flagai/model/tools/lora/prepare_lora.py
+flagai/model/tools/lora/tuners/__init__.py
+flagai/model/tools/lora/tuners/lora.py
+flagai/model/tools/lora/utils/__init__.py
+flagai/model/tools/lora/utils/config.py
+flagai/model/tools/lora/utils/other.py
+flagai/model/tools/lora/utils/save_and_load.py
 flagai/model/vision/__init__.py
 flagai/model/vision/helpers.py
 flagai/model/vision/swinv1.py
 flagai/model/vision/swinv2.py
 flagai/model/vision/vit.py
 flagai/model/vision/layers/__init__.py
 flagai/model/vision/layers/activations.py
```

### Comparing `flagai-1.7.1/setup.py` & `flagai-1.7.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright © 2022 BAAI. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License")
 from setuptools import find_packages, setup
 
 setup(
     name="flagai",
-    version="v1.7.1",
+    version="v1.7.2",
     description="FlagAI aims to help researchers and developers to freely train and test large-scale models for NLP/CV/VL tasks.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="FlagAI-Open",
     author_email="open@baai.ac.cn",
     url="https://github.com/FlagAI-Open/FlagAI",
     packages=find_packages(exclude="tests"),  # same as name
@@ -22,15 +22,15 @@
         'boto3==1.21.42',
         'pandas==1.3.5',
         'jieba==0.42.1',
         'scikit-learn==1.0.2',
         'tensorboard==2.9.0',
         'transformers==4.20.1',
         'datasets==2.0.0',
-        'setuptools==66.0.0',
+        'setuptools==59.5.0',
         'protobuf==3.19.6',
         'ftfy == 6.1.1',
         'Pillow >= 9.3.0',
         'einops == 0.3.0',
         'diffusers == 0.7.2',
         'pytorch-lightning == 1.6.5',
         'taming-transformers-rom1504 == 0.0.6',
```

### Comparing `flagai-1.7.1/tests/bak_test_superglue.py` & `flagai-1.7.2/tests/bak_test_superglue.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/tests/bak_test_t5_ch.py` & `flagai-1.7.2/tests/bak_test_t5_ch.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/tests/test_autoloader.py` & `flagai-1.7.2/tests/test_autoloader.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/tests/test_bert.py` & `flagai-1.7.2/tests/test_bert.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/tests/test_glm_large_ch.py` & `flagai-1.7.2/tests/test_glm_large_ch.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/tests/test_glm_seq2seq.py` & `flagai-1.7.2/tests/test_glm_seq2seq.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/tests/test_gpt2_ch.py` & `flagai-1.7.2/tests/test_gpt2_ch.py`

 * *Files identical despite different names*

### Comparing `flagai-1.7.1/tests/test_tokenizer.py` & `flagai-1.7.2/tests/test_tokenizer.py`

 * *Files identical despite different names*

