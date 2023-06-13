# Comparing `tmp/funasr-0.5.8.tar.gz` & `tmp/funasr-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.5.8.tar", last modified: Tue Jun  6 03:01:04 2023, max compression
+gzip compressed data, was "funasr-0.6.0.tar", last modified: Mon Jun 12 10:55:59 2023, max compression
```

## Comparing `funasr-0.5.8.tar` & `funasr-0.6.0.tar`

### file list

```diff
@@ -1,424 +1,424 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.255468 funasr-0.5.8/
--rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-06 03:01:04.254976 funasr-0.5.8/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7368 2023-06-05 05:14:38.000000 funasr-0.5.8/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.739719 funasr-0.5.8/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.748545 funasr-0.5.8/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    69546 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    72856 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.5.8/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    12198 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15054 2023-05-23 08:26:46.000000 funasr-0.5.8/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.8/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17699 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7276 2023-05-31 06:20:29.000000 funasr-0.5.8/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.751543 funasr-0.5.8/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.5.8/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14060 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.753164 funasr-0.5.8/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.754131 funasr-0.5.8/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 01:45:40.000000 funasr-0.5.8/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.755368 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10367 2023-05-30 04:41:21.000000 funasr-0.5.8/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.757240 funasr-0.5.8/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.8/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.757610 funasr-0.5.8/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.5.8/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.758888 funasr-0.5.8/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.760575 funasr-0.5.8/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.8/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.796474 funasr-0.5.8/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.8/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.798549 funasr-0.5.8/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.8/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.799081 funasr-0.5.8/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.8/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.801403 funasr-0.5.8/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.5.8/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.802008 funasr-0.5.8/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.8/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.804010 funasr-0.5.8/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.805221 funasr-0.5.8/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.808367 funasr-0.5.8/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.809002 funasr-0.5.8/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.810737 funasr-0.5.8/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.822699 funasr-0.5.8/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.8/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.905702 funasr-0.5.8/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.8/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-05-30 08:47:02.000000 funasr-0.5.8/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19490 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31165 2023-05-31 06:20:29.000000 funasr-0.5.8/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.927574 funasr-0.5.8/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.8/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.936368 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-05 05:14:24.000000 funasr-0.5.8/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.961525 funasr-0.5.8/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9122 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-05-31 06:20:29.000000 funasr-0.5.8/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.973345 funasr-0.5.8/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.975604 funasr-0.5.8/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.980310 funasr-0.5.8/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.982443 funasr-0.5.8/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.008282 funasr-0.5.8/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.012478 funasr-0.5.8/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.053830 funasr-0.5.8/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.061987 funasr-0.5.8/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.106101 funasr-0.5.8/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.8/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.111600 funasr-0.5.8/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.8/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.8/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.117013 funasr-0.5.8/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.8/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.8/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.8/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.121616 funasr-0.5.8/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.122973 funasr-0.5.8/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.126792 funasr-0.5.8/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21445 2023-05-25 08:06:43.000000 funasr-0.5.8/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.130404 funasr-0.5.8/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.131802 funasr-0.5.8/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.132618 funasr-0.5.8/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.137065 funasr-0.5.8/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.8/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.141165 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.143916 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.149218 funasr-0.5.8/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.154695 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.159566 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.5.8/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.162506 funasr-0.5.8/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.164054 funasr-0.5.8/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.169139 funasr-0.5.8/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.5.8/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53365 2023-05-24 02:58:26.000000 funasr-0.5.8/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21367 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.172180 funasr-0.5.8/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.179046 funasr-0.5.8/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.8/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.190855 funasr-0.5.8/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.5.8/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.8/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-05-30 08:47:02.000000 funasr-0.5.8/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.235826 funasr-0.5.8/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.8/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.8/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-05-30 09:05:58.000000 funasr-0.5.8/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.8/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.8/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.8/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10094 2023-05-30 04:41:21.000000 funasr-0.5.8/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.8/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.5.8/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.8/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.8/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-06 03:00:01.000000 funasr-0.5.8/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:03.740548 funasr-0.5.8/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13363 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-06 03:01:03.000000 funasr-0.5.8/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-06 03:01:04.255700 funasr-0.5.8/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-05-30 04:55:34.000000 funasr-0.5.8/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-06 03:01:04.251781 funasr-0.5.8/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.8/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.8/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.8/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.8/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.8/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.8/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.766352 funasr-0.6.0/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-12 10:55:59.766129 funasr-0.6.0/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7368 2023-06-05 05:14:38.000000 funasr-0.6.0/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.419936 funasr-0.6.0/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.431173 funasr-0.6.0/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    69546 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    72856 2023-06-12 10:51:43.000000 funasr-0.6.0/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.0/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    12198 2023-05-25 08:06:43.000000 funasr-0.6.0/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15054 2023-05-23 08:26:46.000000 funasr-0.6.0/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.6.0/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17699 2023-05-25 08:06:43.000000 funasr-0.6.0/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7276 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.435433 funasr-0.6.0/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.0/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14060 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.438191 funasr-0.6.0/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.6.0/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.440462 funasr-0.6.0/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.442362 funasr-0.6.0/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10367 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.446014 funasr-0.6.0/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.0/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.0/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.0/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.6.0/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.446680 funasr-0.6.0/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.6.0/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.563206 funasr-0.6.0/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.0/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.599401 funasr-0.6.0/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.0/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.0/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.601526 funasr-0.6.0/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.0/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.0/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.604698 funasr-0.6.0/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.0/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.0/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.605711 funasr-0.6.0/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.0/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.608899 funasr-0.6.0/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.0/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.609734 funasr-0.6.0/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.0/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.613323 funasr-0.6.0/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.614827 funasr-0.6.0/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.618074 funasr-0.6.0/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.6.0/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.619665 funasr-0.6.0/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.6.0/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.623317 funasr-0.6.0/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.634022 funasr-0.6.0/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.6.0/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.640845 funasr-0.6.0/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.6.0/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.6.0/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.6.0/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19490 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31797 2023-06-12 10:54:04.000000 funasr-0.6.0/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.679488 funasr-0.6.0/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.0/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.0/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.0/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.681629 funasr-0.6.0/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.0/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.6.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.685040 funasr-0.6.0/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9122 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.686022 funasr-0.6.0/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.0/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.0/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.687040 funasr-0.6.0/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.0/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.688188 funasr-0.6.0/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.688725 funasr-0.6.0/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.690628 funasr-0.6.0/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.691307 funasr-0.6.0/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.698239 funasr-0.6.0/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.0/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.701476 funasr-0.6.0/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.0/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.705351 funasr-0.6.0/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.0/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.708930 funasr-0.6.0/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.0/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.0/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.712449 funasr-0.6.0/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.0/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.0/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.0/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.0/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.714601 funasr-0.6.0/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.716524 funasr-0.6.0/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.718340 funasr-0.6.0/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21445 2023-05-25 08:06:43.000000 funasr-0.6.0/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.719492 funasr-0.6.0/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.719753 funasr-0.6.0/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.0/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.719968 funasr-0.6.0/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.0/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.720671 funasr-0.6.0/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.0/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.721942 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.724045 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.726699 funasr-0.6.0/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.728414 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.736055 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.6.0/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.739217 funasr-0.6.0/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.740369 funasr-0.6.0/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.744797 funasr-0.6.0/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.6.0/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53365 2023-05-24 02:58:26.000000 funasr-0.6.0/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21367 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.747631 funasr-0.6.0/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.750689 funasr-0.6.0/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.0/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.752539 funasr-0.6.0/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.6.0/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.0/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.762816 funasr-0.6.0/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.6.0/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.0/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.0/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.0/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.0/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.0/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10094 2023-06-06 13:50:59.000000 funasr-0.6.0/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.0/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.0/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.6.0/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.0/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-12 10:54:57.000000 funasr-0.6.0/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.420851 funasr-0.6.0/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-12 10:55:59.000000 funasr-0.6.0/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13363 2023-06-12 10:55:59.000000 funasr-0.6.0/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-12 10:55:59.000000 funasr-0.6.0/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-12 10:55:59.000000 funasr-0.6.0/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-12 10:55:59.000000 funasr-0.6.0/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-12 10:55:59.766414 funasr-0.6.0/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-06-06 13:50:59.000000 funasr-0.6.0/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-12 10:55:59.765630 funasr-0.6.0/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.6.0/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.6.0/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.0/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.0/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.6.0/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.6.0/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.5.8/PKG-INFO` & `funasr-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.8
+Version: 0.6.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.8 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.0 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
```

### Comparing `funasr-0.5.8/README.md` & `funasr-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.6.0/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/asr_infer.py` & `funasr-0.6.0/funasr/bin/asr_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/asr_inference_launch.py` & `funasr-0.6.0/funasr/bin/asr_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/asr_train.py` & `funasr-0.6.0/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/build_trainer.py` & `funasr-0.6.0/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/data2vec_train.py` & `funasr-0.6.0/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/diar_infer.py` & `funasr-0.6.0/funasr/bin/diar_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/diar_inference_launch.py` & `funasr-0.6.0/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/diar_train.py` & `funasr-0.6.0/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/lm_inference_launch.py` & `funasr-0.6.0/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/lm_train.py` & `funasr-0.6.0/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/punc_infer.py` & `funasr-0.6.0/funasr/bin/punc_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/punc_inference_launch.py` & `funasr-0.6.0/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/punc_train.py` & `funasr-0.6.0/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/sa_asr_train.py` & `funasr-0.6.0/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/sv_infer.py` & `funasr-0.6.0/funasr/bin/sv_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/sv_inference_launch.py` & `funasr-0.6.0/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/tokenize_text.py` & `funasr-0.6.0/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/tp_infer.py` & `funasr-0.6.0/funasr/bin/tp_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/tp_inference_launch.py` & `funasr-0.6.0/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/train.py` & `funasr-0.6.0/funasr/bin/train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/vad_infer.py` & `funasr-0.6.0/funasr/bin/vad_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/bin/vad_inference_launch.py` & `funasr-0.6.0/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_args.py` & `funasr-0.6.0/funasr/build_utils/build_args.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_asr_model.py` & `funasr-0.6.0/funasr/build_utils/build_asr_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_dataloader.py` & `funasr-0.6.0/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_diar_model.py` & `funasr-0.6.0/funasr/build_utils/build_diar_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_distributed.py` & `funasr-0.6.0/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_lm_model.py` & `funasr-0.6.0/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_model.py` & `funasr-0.6.0/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_optimizer.py` & `funasr-0.6.0/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_pretrain_model.py` & `funasr-0.6.0/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_punc_model.py` & `funasr-0.6.0/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_scheduler.py` & `funasr-0.6.0/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_trainer.py` & `funasr-0.6.0/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/build_utils/build_vad_model.py` & `funasr-0.6.0/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/collate_fn.py` & `funasr-0.6.0/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/dataset.py` & `funasr-0.6.0/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/iterable_dataset.py` & `funasr-0.6.0/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.6.0/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.6.0/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.6.0/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/dataset.py` & `funasr-0.6.0/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.6.0/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.6.0/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.6.0/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.6.0/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.6.0/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.6.0/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/ms_dataset.py` & `funasr-0.6.0/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/datasets/preprocessor.py` & `funasr-0.6.0/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/export_model.py` & `funasr-0.6.0/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/CT_Transformer.py` & `funasr-0.6.0/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/__init__.py` & `funasr-0.6.0/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.6.0/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.6.0/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.6.0/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/e2e_vad.py` & `funasr-0.6.0/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.6.0/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.6.0/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.6.0/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/modules/decoder_layer.py` & `funasr-0.6.0/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/modules/encoder_layer.py` & `funasr-0.6.0/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/modules/feedforward.py` & `funasr-0.6.0/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/modules/multihead_att.py` & `funasr-0.6.0/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/models/predictor/cif.py` & `funasr-0.6.0/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/test/test_onnx.py` & `funasr-0.6.0/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/test/test_onnx_punc.py` & `funasr-0.6.0/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.6.0/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/test/test_onnx_vad.py` & `funasr-0.6.0/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/export/utils/torch_function.py` & `funasr-0.6.0/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/fileio/datadir_writer.py` & `funasr-0.6.0/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/fileio/npy_scp.py` & `funasr-0.6.0/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/fileio/rand_gen_dataset.py` & `funasr-0.6.0/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/fileio/read_text.py` & `funasr-0.6.0/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/fileio/sound_scp.py` & `funasr-0.6.0/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/iterators/chunk_iter_factory.py` & `funasr-0.6.0/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/iterators/multiple_iter_factory.py` & `funasr-0.6.0/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/iterators/sequence_iter_factory.py` & `funasr-0.6.0/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/complex_utils.py` & `funasr-0.6.0/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/global_mvn.py` & `funasr-0.6.0/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/label_aggregation.py` & `funasr-0.6.0/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/log_mel.py` & `funasr-0.6.0/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/mask_along_axis.py` & `funasr-0.6.0/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/sinc_conv.py` & `funasr-0.6.0/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/stft.py` & `funasr-0.6.0/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/time_warp.py` & `funasr-0.6.0/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/layers/utterance_mvn.py` & `funasr-0.6.0/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/losses/label_smoothing_loss.py` & `funasr-0.6.0/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/main_funcs/average_nbest_models.py` & `funasr-0.6.0/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.6.0/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/main_funcs/collect_stats.py` & `funasr-0.6.0/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/main_funcs/pack_funcs.py` & `funasr-0.6.0/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/ctc.py` & `funasr-0.6.0/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/data2vec.py` & `funasr-0.6.0/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/decoder/contextual_decoder.py` & `funasr-0.6.0/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/decoder/rnn_decoder.py` & `funasr-0.6.0/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.6.0/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/decoder/sanm_decoder.py` & `funasr-0.6.0/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/decoder/sv_decoder.py` & `funasr-0.6.0/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/decoder/transformer_decoder.py` & `funasr-0.6.0/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_asr.py` & `funasr-0.6.0/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_asr_common.py` & `funasr-0.6.0/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.6.0/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_asr_mfcca.py` & `funasr-0.6.0/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_asr_paraformer.py` & `funasr-0.6.0/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_asr_transducer.py` & `funasr-0.6.0/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.6.0/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_diar_sond.py` & `funasr-0.6.0/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_sa_asr.py` & `funasr-0.6.0/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_sv.py` & `funasr-0.6.0/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_tp.py` & `funasr-0.6.0/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_uni_asr.py` & `funasr-0.6.0/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/e2e_vad.py` & `funasr-0.6.0/funasr/models/e2e_vad.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,16 @@
         self.speech_noise_thres = self.vad_opts.speech_noise_thres
         self.scores = None
         self.max_time_out = False
         self.decibel = []
         self.data_buf = None
         self.data_buf_all = None
         self.waveform = None
-        self.ResetDetection()
         self.frontend = frontend
+        self.last_drop_frames = 0
 
     def AllResetDetection(self):
         self.data_buf_start_frame = 0
         self.frm_cnt = 0
         self.latest_confirmed_speech_frame = 0
         self.lastest_confirmed_silence_frame = -1
         self.continous_silence_frame_count = 0
@@ -278,27 +278,36 @@
         self.speech_noise_thres = self.vad_opts.speech_noise_thres
         self.scores = None
         self.max_time_out = False
         self.decibel = []
         self.data_buf = None
         self.data_buf_all = None
         self.waveform = None
-        self.ResetDetection()
+        self.last_drop_frames = 0
+        self.windows_detector.Reset()
 
     def ResetDetection(self):
         self.continous_silence_frame_count = 0
         self.latest_confirmed_speech_frame = 0
         self.lastest_confirmed_silence_frame = -1
         self.confirmed_start_frame = -1
         self.confirmed_end_frame = -1
         self.vad_state_machine = VadStateMachine.kVadInStateStartPointNotDetected
         self.windows_detector.Reset()
         self.sil_frame = 0
         self.frame_probs = []
 
+        assert self.output_data_buf[-1].contain_seg_end_point == True
+        drop_frames = int(self.output_data_buf[-1].end_ms / self.vad_opts.frame_in_ms)
+        real_drop_frames = drop_frames - self.last_drop_frames
+        self.last_drop_frames = drop_frames
+        self.data_buf_all = self.data_buf_all[real_drop_frames * int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):]
+        self.decibel = self.decibel[real_drop_frames:]
+        self.scores = self.scores[:, real_drop_frames:, :]
+
     def ComputeDecibel(self) -> None:
         frame_sample_length = int(self.vad_opts.frame_length_ms * self.vad_opts.sample_rate / 1000)
         frame_shift_length = int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000)
         if self.data_buf_all is None:
             self.data_buf_all = self.waveform[0]  # self.data_buf is pointed to self.waveform[0]
             self.data_buf = self.data_buf_all
         else:
@@ -318,15 +327,15 @@
         else:
             self.scores = torch.cat((self.scores, scores), dim=1)
 
     def PopDataBufTillFrame(self, frame_idx: int) -> None:  # need check again
         while self.data_buf_start_frame < frame_idx:
             if len(self.data_buf) >= int(self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):
                 self.data_buf_start_frame += 1
-                self.data_buf = self.data_buf_all[self.data_buf_start_frame * int(
+                self.data_buf = self.data_buf_all[(self.data_buf_start_frame - self.last_drop_frames) * int(
                     self.vad_opts.frame_in_ms * self.vad_opts.sample_rate / 1000):]
 
     def PopDataToOutputBuf(self, start_frm: int, frm_cnt: int, first_frm_is_start_point: bool,
                            last_frm_is_end_point: bool, end_point_is_sent_end: bool) -> None:
         self.PopDataBufTillFrame(start_frm)
         expected_sample_number = int(frm_cnt * self.vad_opts.sample_rate * self.vad_opts.frame_in_ms / 1000)
         if last_frm_is_end_point:
@@ -539,25 +548,25 @@
         return segments, in_cache
 
     def DetectCommonFrames(self) -> int:
         if self.vad_state_machine == VadStateMachine.kVadInStateEndPointDetected:
             return 0
         for i in range(self.vad_opts.nn_eval_block_size - 1, -1, -1):
             frame_state = FrameState.kFrameStateInvalid
-            frame_state = self.GetFrameState(self.frm_cnt - 1 - i)
+            frame_state = self.GetFrameState(self.frm_cnt - 1 - i - self.last_drop_frames)
             self.DetectOneFrame(frame_state, self.frm_cnt - 1 - i, False)
 
         return 0
 
     def DetectLastFrames(self) -> int:
         if self.vad_state_machine == VadStateMachine.kVadInStateEndPointDetected:
             return 0
         for i in range(self.vad_opts.nn_eval_block_size - 1, -1, -1):
             frame_state = FrameState.kFrameStateInvalid
-            frame_state = self.GetFrameState(self.frm_cnt - 1 - i)
+            frame_state = self.GetFrameState(self.frm_cnt - 1 - i - self.last_drop_frames)
             if i != 0:
                 self.DetectOneFrame(frame_state, self.frm_cnt - 1 - i, False)
             else:
                 self.DetectOneFrame(frame_state, self.frm_cnt - 1, True)
 
         return 0
```

### Comparing `funasr-0.5.8/funasr/models/encoder/conformer_encoder.py` & `funasr-0.6.0/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.6.0/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.6.0/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.6.0/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.6.0/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.6.0/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.6.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.6.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.6.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.6.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.6.0/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/rnn_encoder.py` & `funasr-0.6.0/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/sanm_encoder.py` & `funasr-0.6.0/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/encoder/transformer_encoder.py` & `funasr-0.6.0/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/frontend/default.py` & `funasr-0.6.0/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.6.0/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/frontend/fused.py` & `funasr-0.6.0/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/frontend/s3prl.py` & `funasr-0.6.0/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/frontend/wav_frontend.py` & `funasr-0.6.0/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.6.0/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/frontend/windowing.py` & `funasr-0.6.0/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/joint_net/joint_network.py` & `funasr-0.6.0/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/pooling/statistic_pooling.py` & `funasr-0.6.0/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.6.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/predictor/cif.py` & `funasr-0.6.0/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/preencoder/linear.py` & `funasr-0.6.0/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/preencoder/sinc.py` & `funasr-0.6.0/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/seq_rnn_lm.py` & `funasr-0.6.0/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/specaug/specaug.py` & `funasr-0.6.0/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/target_delay_transformer.py` & `funasr-0.6.0/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/transformer_lm.py` & `funasr-0.6.0/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/models/vad_realtime_transformer.py` & `funasr-0.6.0/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/add_sos_eos.py` & `funasr-0.6.0/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/attention.py` & `funasr-0.6.0/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.6.0/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.6.0/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/beam_search/beam_search.py` & `funasr-0.6.0/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.6.0/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.6.0/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/data2vec/data_utils.py` & `funasr-0.6.0/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/data2vec/ema_module.py` & `funasr-0.6.0/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.6.0/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/data2vec/quant_noise.py` & `funasr-0.6.0/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/data2vec/utils.py` & `funasr-0.6.0/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.6.0/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/dynamic_conv.py` & `funasr-0.6.0/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/dynamic_conv2d.py` & `funasr-0.6.0/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/e2e_asr_common.py` & `funasr-0.6.0/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/eend_ola/encoder.py` & `funasr-0.6.0/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.6.0/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/embedding.py` & `funasr-0.6.0/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/frontends/beamformer.py` & `funasr-0.6.0/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.6.0/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.6.0/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/frontends/feature_transform.py` & `funasr-0.6.0/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/frontends/frontend.py` & `funasr-0.6.0/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/frontends/mask_estimator.py` & `funasr-0.6.0/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/layer_norm.py` & `funasr-0.6.0/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/lightconv.py` & `funasr-0.6.0/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/lightconv2d.py` & `funasr-0.6.0/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/mask.py` & `funasr-0.6.0/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/multi_layer_conv.py` & `funasr-0.6.0/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/nets_utils.py` & `funasr-0.6.0/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/positionwise_feed_forward.py` & `funasr-0.6.0/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/repeat.py` & `funasr-0.6.0/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/rnn/argument.py` & `funasr-0.6.0/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/rnn/attentions.py` & `funasr-0.6.0/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/rnn/decoders.py` & `funasr-0.6.0/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/rnn/encoders.py` & `funasr-0.6.0/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/scorers/ctc.py` & `funasr-0.6.0/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.6.0/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/scorers/length_bonus.py` & `funasr-0.6.0/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/scorers/scorer_interface.py` & `funasr-0.6.0/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.6.0/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.6.0/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/streaming_utils/utils.py` & `funasr-0.6.0/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/subsampling.py` & `funasr-0.6.0/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/modules/subsampling_without_posenc.py` & `funasr-0.6.0/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/optimizers/fairseq_adam.py` & `funasr-0.6.0/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/optimizers/sgd.py` & `funasr-0.6.0/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/demo.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/libtorch/setup.py` & `funasr-0.6.0/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.6.0/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/samplers/build_batch_sampler.py` & `funasr-0.6.0/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/samplers/folded_batch_sampler.py` & `funasr-0.6.0/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/samplers/length_batch_sampler.py` & `funasr-0.6.0/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.6.0/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.6.0/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.6.0/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/schedulers/abs_scheduler.py` & `funasr-0.6.0/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/schedulers/noam_lr.py` & `funasr-0.6.0/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.6.0/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/schedulers/warmup_lr.py` & `funasr-0.6.0/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/abs_task.py` & `funasr-0.6.0/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/asr.py` & `funasr-0.6.0/funasr/tasks/asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/data2vec.py` & `funasr-0.6.0/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/diar.py` & `funasr-0.6.0/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/lm.py` & `funasr-0.6.0/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/punctuation.py` & `funasr-0.6.0/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/sa_asr.py` & `funasr-0.6.0/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/sv.py` & `funasr-0.6.0/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/tasks/vad.py` & `funasr-0.6.0/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/build_tokenizer.py` & `funasr-0.6.0/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/char_tokenizer.py` & `funasr-0.6.0/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/cleaner.py` & `funasr-0.6.0/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/korean_cleaner.py` & `funasr-0.6.0/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/phoneme_tokenizer.py` & `funasr-0.6.0/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.6.0/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/token_id_converter.py` & `funasr-0.6.0/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/text/word_tokenizer.py` & `funasr-0.6.0/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.6.0/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/torch_utils/device_funcs.py` & `funasr-0.6.0/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/torch_utils/forward_adaptor.py` & `funasr-0.6.0/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/torch_utils/initialize.py` & `funasr-0.6.0/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.6.0/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/torch_utils/model_summary.py` & `funasr-0.6.0/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/torch_utils/recursive_op.py` & `funasr-0.6.0/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/train/abs_model.py` & `funasr-0.6.0/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/train/class_choices.py` & `funasr-0.6.0/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/train/distributed_utils.py` & `funasr-0.6.0/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/train/reporter.py` & `funasr-0.6.0/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/train/trainer.py` & `funasr-0.6.0/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/asr_env_checking.py` & `funasr-0.6.0/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/asr_utils.py` & `funasr-0.6.0/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/build_dataclass.py` & `funasr-0.6.0/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/cli_utils.py` & `funasr-0.6.0/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/compute_eer.py` & `funasr-0.6.0/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/compute_min_dcf.py` & `funasr-0.6.0/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/compute_wer.py` & `funasr-0.6.0/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/config_argparse.py` & `funasr-0.6.0/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/get_default_kwargs.py` & `funasr-0.6.0/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/griffin_lim.py` & `funasr-0.6.0/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/job_runner.py` & `funasr-0.6.0/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/misc.py` & `funasr-0.6.0/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/modelscope_param.py` & `funasr-0.6.0/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/modelscope_utils.py` & `funasr-0.6.0/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/nested_dict_action.py` & `funasr-0.6.0/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/postprocess_utils.py` & `funasr-0.6.0/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/prepare_data.py` & `funasr-0.6.0/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/sized_dict.py` & `funasr-0.6.0/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/timestamp_tools.py` & `funasr-0.6.0/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/types.py` & `funasr-0.6.0/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/vad_utils.py` & `funasr-0.6.0/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr/utils/wav_utils.py` & `funasr-0.6.0/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr.egg-info/PKG-INFO` & `funasr-0.6.0/funasr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.8
+Version: 0.6.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.8 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.0 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
```

### Comparing `funasr-0.5.8/funasr.egg-info/SOURCES.txt` & `funasr-0.6.0/funasr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/funasr.egg-info/requires.txt` & `funasr-0.6.0/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/setup.py` & `funasr-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/tests/test_asr_inference_pipeline.py` & `funasr-0.6.0/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.6.0/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/tests/test_lm_pipeline.py` & `funasr-0.6.0/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/tests/test_punctuation_pipeline.py` & `funasr-0.6.0/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/tests/test_sv_inference_pipeline.py` & `funasr-0.6.0/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.8/tests/test_vad_inference_pipeline.py` & `funasr-0.6.0/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

