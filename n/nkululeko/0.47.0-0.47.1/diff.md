# Comparing `tmp/nkululeko-0.47.0.tar.gz` & `tmp/nkululeko-0.47.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.47.0.tar", last modified: Thu May 25 16:48:21 2023, max compression
+gzip compressed data, was "nkululeko-0.47.1.tar", last modified: Tue Jun 13 14:42:07 2023, max compression
```

## Comparing `nkululeko-0.47.0.tar` & `nkululeko-0.47.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-25 16:48:21.729026 nkululeko-0.47.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6217 2023-05-25 16:47:33.000000 nkululeko-0.47.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.47.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17239 2023-05-25 16:48:21.729026 nkululeko-0.47.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10469 2023-05-11 10:04:04.000000 nkululeko-0.47.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-25 16:48:21.725026 nkululeko-0.47.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.47.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.47.0/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.47.0/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.47.0/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.47.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-05-25 16:46:01.000000 nkululeko-0.47.0/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-23 12:23:55.000000 nkululeko-0.47.0/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.47.0/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.47.0/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.47.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.47.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20319 2023-05-23 12:09:53.000000 nkululeko-0.47.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.47.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.47.0/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.47.0/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.47.0/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.47.0/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.47.0/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.47.0/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.47.0/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.47.0/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2130 2023-05-23 11:53:38.000000 nkululeko-0.47.0/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.47.0/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.47.0/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.47.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.47.0/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19509 2023-05-25 16:45:46.000000 nkululeko-0.47.0/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.47.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.47.0/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.47.0/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.47.0/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.47.0/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.47.0/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.47.0/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.47.0/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.47.0/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.47.0/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.47.0/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.47.0/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.47.0/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.47.0/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.47.0/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.47.0/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.47.0/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.47.0/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.47.0/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.47.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.47.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.47.0/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.47.0/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.47.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.47.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.47.0/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.47.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.47.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8967 2023-05-23 11:38:09.000000 nkululeko-0.47.0/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-25 16:48:21.729026 nkululeko-0.47.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17239 2023-05-25 16:48:21.000000 nkululeko-0.47.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1594 2023-05-25 16:48:21.000000 nkululeko-0.47.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-25 16:48:21.000000 nkululeko-0.47.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-25 16:48:21.000000 nkululeko-0.47.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-25 16:48:21.000000 nkululeko-0.47.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.47.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-05-25 16:48:21.729026 nkululeko-0.47.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.47.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-13 14:42:07.844685 nkululeko-0.47.1/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6308 2023-06-13 14:23:01.000000 nkululeko-0.47.1/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.47.1/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18034 2023-06-13 14:42:07.844685 nkululeko-0.47.1/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.47.1/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-13 14:42:07.844685 nkululeko-0.47.1/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.47.1/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.47.1/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.47.1/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.47.1/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.47.1/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-13 14:22:23.000000 nkululeko-0.47.1/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-23 12:23:55.000000 nkululeko-0.47.1/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.47.1/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.47.1/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.47.1/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.47.1/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20319 2023-05-23 12:09:53.000000 nkululeko-0.47.1/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.47.1/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.47.1/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.47.1/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.47.1/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.47.1/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.47.1/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.47.1/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2871 2023-06-13 14:22:08.000000 nkululeko-0.47.1/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.47.1/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2130 2023-05-23 11:53:38.000000 nkululeko-0.47.1/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.47.1/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.47.1/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.47.1/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.47.1/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19509 2023-05-25 16:45:46.000000 nkululeko-0.47.1/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.47.1/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.47.1/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.47.1/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.47.1/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.47.1/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.47.1/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.47.1/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.47.1/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.47.1/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.47.1/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.47.1/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.47.1/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.47.1/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.47.1/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.47.1/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.47.1/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.47.1/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.47.1/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.47.1/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.47.1/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.47.1/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.47.1/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.47.1/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.47.1/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.47.1/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.47.1/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.47.1/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.47.1/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8967 2023-05-23 11:38:09.000000 nkululeko-0.47.1/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-13 14:42:07.844685 nkululeko-0.47.1/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18034 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1594 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.47.1/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-13 14:42:07.844685 nkululeko-0.47.1/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.47.1/setup.py
```

### Comparing `nkululeko-0.47.0/CHANGELOG.md` & `nkululeko-0.47.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.47.1
+--------------
+* enabled feature storage format csv for opensmile features
+
 Version 0.47.0
 --------------
 * added praat speech rate features
 
 Version 0.46.0
 --------------
 * added warnings for non-existent parameters
```

### Comparing `nkululeko-0.47.0/LICENSE` & `nkululeko-0.47.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/PKG-INFO` & `nkululeko-0.47.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.47.0
+Version: 0.47.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,58 +16,59 @@
 
 # Nkululeko
 * [Overview](#overview)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Hello World](#hello-world-example)
 * [Licence](#licence)
-
+ 
 ## Overview
 A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
-The idea is to have a framework (based on e.g. sklearn and torch) that can be used by people not being experienced programmers as they mainly have to adapt an initialization parameter file per experiment.
+The idea is to have a framework (based on e.g. sklearn and torch) that can be used to rapidly and automatically analyse and investigate audio data automatically.
 
+* New [We started a slack channel to discuss issues related to nkululeko](https://join.slack.com/t/nkululekoworkspace/shared_invite/zt-1wtvbxtwz-P5YoRJq8whxKSee86ebhJg). Please click the link if interested in contributing.
 * The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
-* Below is a [Hello World example](#helloworld) that should set you up fastly.
+* Below is a [Hello World example](#helloworld) that should set you up fastly, also on [Google Colab](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
 
 ### Confusion matrix
 Per default, Nkululeko displays results as a confusion matrix using binning with regression.
 
-<img src="images/conf_mat.png" width="500px"/>
+<img src="meta/images/conf_mat.png" width="500px"/>
 
 ### Epoch progression
 The point when overfitting starts can sometimes be seen by looking at the results per epoch:
 
-<img src="images/epoch_progression.png" width="500px"/>
+<img src="meta/images/epoch_progression.png" width="500px"/>
 
 ### Feature importance
 Using the *explore* interface, Nkululeko analyses the importance of acoustic features:
  
-<img src="images/feat_importance.png" width="500px"/>
+<img src="meta/images/feat_importance.png" width="500px"/>
 
 ### Feature distribution
 And can show the distribution of specific features per category:
 
-<img src="images/feat_dist.png" width="500px"/>
+<img src="meta/images/feat_dist.png" width="500px"/>
 
 ### t-SNE plots
 A t-SNE plot can give you an estimate wether your acoustic features are useful at all:
 
-<img src="images/tsne.png" width="500px"/>
+<img src="meta/images/tsne.png" width="500px"/>
 
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
-<img src="images/data_plot.png" width="500px"/>
+<img src="meta/images/data_plot.png" width="500px"/>
 
 ## Installation
 
 Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
@@ -142,15 +143,15 @@
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
  * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
-![sketch](images/class_diagram.png)
+![sketch](meta/images/class_diagram.png)
 
 Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
@@ -160,15 +161,16 @@
 * use a generic main python file (like my_experiment.py), 
 * adapt the path to your nkululeko src 
 * and then adapt an .ini file (again fitting at least the paths to src and data)
   
 Here's [an overview of the ini-file options](./ini_file.md)
 
 ### <a name="helloworld">Hello World example</a>
-* NEW: [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
+* NEW: [Here's a Google colab that runs this example out-of-the-box](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and here is the same [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
+* [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * Set up Python on your computer, version >= 3.6
 * Open a terminal/commandline/console window
 * Test python by typing ```python```, python should start with version >3 (NOT 2!). You can leave the Python Interpreter by typing *exit()*
 * Create a folder on your computer for this example, let's call it `nkulu_work`
 * Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (`nkulu_work`)
 * Make sure the folder is called "emodb" and does contain the database files directly (not box-in-a-box)
 * Also, in the `nkulu_work` folder: 
@@ -208,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.47.1
+--------------
+* enabled feature storage format csv for opensmile features
+
 Version 0.47.0
 --------------
 * added praat speech rate features
 
 Version 0.46.0
 --------------
 * added warnings for non-existent parameters
```

### Comparing `nkululeko-0.47.0/README.md` & `nkululeko-0.47.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 # Nkululeko
 * [Overview](#overview)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Hello World](#hello-world-example)
 * [Licence](#licence)
-
+ 
 ## Overview
 A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
-The idea is to have a framework (based on e.g. sklearn and torch) that can be used by people not being experienced programmers as they mainly have to adapt an initialization parameter file per experiment.
+The idea is to have a framework (based on e.g. sklearn and torch) that can be used to rapidly and automatically analyse and investigate audio data automatically.
 
+* New [We started a slack channel to discuss issues related to nkululeko](https://join.slack.com/t/nkululekoworkspace/shared_invite/zt-1wtvbxtwz-P5YoRJq8whxKSee86ebhJg). Please click the link if interested in contributing.
 * The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
-* Below is a [Hello World example](#helloworld) that should set you up fastly.
+* Below is a [Hello World example](#helloworld) that should set you up fastly, also on [Google Colab](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
 
 ### Confusion matrix
 Per default, Nkululeko displays results as a confusion matrix using binning with regression.
 
-<img src="images/conf_mat.png" width="500px"/>
+<img src="meta/images/conf_mat.png" width="500px"/>
 
 ### Epoch progression
 The point when overfitting starts can sometimes be seen by looking at the results per epoch:
 
-<img src="images/epoch_progression.png" width="500px"/>
+<img src="meta/images/epoch_progression.png" width="500px"/>
 
 ### Feature importance
 Using the *explore* interface, Nkululeko analyses the importance of acoustic features:
  
-<img src="images/feat_importance.png" width="500px"/>
+<img src="meta/images/feat_importance.png" width="500px"/>
 
 ### Feature distribution
 And can show the distribution of specific features per category:
 
-<img src="images/feat_dist.png" width="500px"/>
+<img src="meta/images/feat_dist.png" width="500px"/>
 
 ### t-SNE plots
 A t-SNE plot can give you an estimate wether your acoustic features are useful at all:
 
-<img src="images/tsne.png" width="500px"/>
+<img src="meta/images/tsne.png" width="500px"/>
 
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
-<img src="images/data_plot.png" width="500px"/>
+<img src="meta/images/data_plot.png" width="500px"/>
 
 ## Installation
 
 Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
@@ -126,15 +127,15 @@
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
  * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
-![sketch](images/class_diagram.png)
+![sketch](meta/images/class_diagram.png)
 
 Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
@@ -144,15 +145,16 @@
 * use a generic main python file (like my_experiment.py), 
 * adapt the path to your nkululeko src 
 * and then adapt an .ini file (again fitting at least the paths to src and data)
   
 Here's [an overview of the ini-file options](./ini_file.md)
 
 ### <a name="helloworld">Hello World example</a>
-* NEW: [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
+* NEW: [Here's a Google colab that runs this example out-of-the-box](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and here is the same [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
+* [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * Set up Python on your computer, version >= 3.6
 * Open a terminal/commandline/console window
 * Test python by typing ```python```, python should start with version >3 (NOT 2!). You can leave the Python Interpreter by typing *exit()*
 * Create a folder on your computer for this example, let's call it `nkulu_work`
 * Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (`nkulu_work`)
 * Make sure the folder is called "emodb" and does contain the database files directly (not box-in-a-box)
 * Also, in the `nkulu_work` folder:
```

### Comparing `nkululeko-0.47.0/nkululeko/augment.py` & `nkululeko-0.47.1/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/augmenter.py` & `nkululeko-0.47.1/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/cacheddataset.py` & `nkululeko-0.47.1/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/dataset.py` & `nkululeko-0.47.1/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/dataset_csv.py` & `nkululeko-0.47.1/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/dataset_ravdess.py` & `nkululeko-0.47.1/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/demo.py` & `nkululeko-0.47.1/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/demo_predictor.py` & `nkululeko-0.47.1/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/experiment.py` & `nkululeko-0.47.1/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/explore.py` & `nkululeko-0.47.1/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_analyser.py` & `nkululeko-0.47.1/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_audmodel.py` & `nkululeko-0.47.1/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.47.1/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_clap.py` & `nkululeko-0.47.1/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_import.py` & `nkululeko-0.47.1/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_mld.py` & `nkululeko-0.47.1/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_opensmile.py` & `nkululeko-0.47.1/nkululeko/feats_opensmile.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         except AttributeError:        
             self.util.error(f'something is wrong with feature level: {self.featlevel}')        
 
 
     def extract(self):
         """Extract the features based on the initialized dataset or re-open them when found on disk."""
         store = self.util.get_path('store')
-        storage = f'{store}{self.name}_{self.featset}.pkl'
+        store_format = self.util.config_val('FEATS', 'store_format', 'pkl')
+        storage = f'{store}{self.name}.{store_format}'
         extract = eval(self.util.config_val('FEATS', 'needs_feature_extraction', 'False'))
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
         if extract or not os.path.isfile(storage) or no_reuse:
             self.util.debug('extracting openSmile features, this might take a while...')
             smile = opensmile.Smile(
             feature_set= self.feature_set,
             feature_level=self.feature_level,
@@ -40,15 +41,15 @@
             if isinstance(self.data_df.index, pd.MultiIndex):
                 self.df = smile.process_index(self.data_df.index)
                 self.df = self.df.set_index(self.data_df.index)
             else:
                 self.df = smile.process_files(self.data_df.index)
                 self.df.index = self.df.index.droplevel(1)
                 self.df.index = self.df.index.droplevel(1)
-            self.df.to_pickle(storage)
+            self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'False'
             except KeyError:
                 pass
         else:
             self.util.debug('reusing extracted OS features.')
             self.df = pd.read_pickle(storage)
```

### Comparing `nkululeko-0.47.0/nkululeko/feats_oxbow.py` & `nkululeko-0.47.1/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_praat.py` & `nkululeko-0.47.1/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_trill.py` & `nkululeko-0.47.1/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feats_wav2vec2.py` & `nkululeko-0.47.1/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feature_extractor.py` & `nkululeko-0.47.1/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/featureset.py` & `nkululeko-0.47.1/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/feinberg_praat.py` & `nkululeko-0.47.1/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/filter_data.py` & `nkululeko-0.47.1/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/loss_ccc.py` & `nkululeko-0.47.1/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/loss_softf1loss.py` & `nkululeko-0.47.1/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model.py` & `nkululeko-0.47.1/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model_cnn.py` & `nkululeko-0.47.1/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model_gmm.py` & `nkululeko-0.47.1/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model_knn.py` & `nkululeko-0.47.1/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model_knn_reg.py` & `nkululeko-0.47.1/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model_mlp.py` & `nkululeko-0.47.1/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model_mlp_regression.py` & `nkululeko-0.47.1/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/model_svm.py` & `nkululeko-0.47.1/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/modelrunner.py` & `nkululeko-0.47.1/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/nkululeko.py` & `nkululeko-0.47.1/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/plots.py` & `nkululeko-0.47.1/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/reporter.py` & `nkululeko-0.47.1/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/runmanager.py` & `nkululeko-0.47.1/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/scaler.py` & `nkululeko-0.47.1/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/syllable_nuclei.py` & `nkululeko-0.47.1/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/test.py` & `nkululeko-0.47.1/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/test_predictor.py` & `nkululeko-0.47.1/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko/util.py` & `nkululeko-0.47.1/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.47.1/nkululeko.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.47.0
+Version: 0.47.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,58 +16,59 @@
 
 # Nkululeko
 * [Overview](#overview)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Hello World](#hello-world-example)
 * [Licence](#licence)
-
+ 
 ## Overview
 A project to detect speaker characteristics by machine learning experiments with a high-level interface.
 
-The idea is to have a framework (based on e.g. sklearn and torch) that can be used by people not being experienced programmers as they mainly have to adapt an initialization parameter file per experiment.
+The idea is to have a framework (based on e.g. sklearn and torch) that can be used to rapidly and automatically analyse and investigate audio data automatically.
 
+* New [We started a slack channel to discuss issues related to nkululeko](https://join.slack.com/t/nkululekoworkspace/shared_invite/zt-1wtvbxtwz-P5YoRJq8whxKSee86ebhJg). Please click the link if interested in contributing.
 * The latest features can be seen in [the ini-file](./ini_file.md) options](./ini_file.md) that are used to control Nkululeko
-* Below is a [Hello World example](#helloworld) that should set you up fastly.
+* Below is a [Hello World example](#helloworld) that should set you up fastly, also on [Google Colab](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
 * [Here's a blog post on how to set up nkululeko on your computer.](http://blog.syntheticspeech.de/2021/08/30/how-to-set-up-your-first-nkululeko-project/)
 * [Here's a slide presentation about nkululeko](docs/nkululeko.pdf)
 * [Here's a video presentation about nkululeko](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * [Here's the 2022 LREC article on nkululeko](http://felix.syntheticspeech.de/publications/Nkululeko_LREC.pdf)
 
 Here are some examples of typical output:
 
 ### Confusion matrix
 Per default, Nkululeko displays results as a confusion matrix using binning with regression.
 
-<img src="images/conf_mat.png" width="500px"/>
+<img src="meta/images/conf_mat.png" width="500px"/>
 
 ### Epoch progression
 The point when overfitting starts can sometimes be seen by looking at the results per epoch:
 
-<img src="images/epoch_progression.png" width="500px"/>
+<img src="meta/images/epoch_progression.png" width="500px"/>
 
 ### Feature importance
 Using the *explore* interface, Nkululeko analyses the importance of acoustic features:
  
-<img src="images/feat_importance.png" width="500px"/>
+<img src="meta/images/feat_importance.png" width="500px"/>
 
 ### Feature distribution
 And can show the distribution of specific features per category:
 
-<img src="images/feat_dist.png" width="500px"/>
+<img src="meta/images/feat_dist.png" width="500px"/>
 
 ### t-SNE plots
 A t-SNE plot can give you an estimate wether your acoustic features are useful at all:
 
-<img src="images/tsne.png" width="500px"/>
+<img src="meta/images/tsne.png" width="500px"/>
 
 ### Data distribution
 Sometimes you only want to take a look at your data:
 
-<img src="images/data_plot.png" width="500px"/>
+<img src="meta/images/data_plot.png" width="500px"/>
 
 ## Installation
 
 Create and activate a virtual Python environment and simply run
 ```
 pip install nkululeko
 ```
@@ -142,15 +143,15 @@
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
  * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
-![sketch](images/class_diagram.png)
+![sketch](meta/images/class_diagram.png)
 
 Currently, the following linear classifiers are implemented (integrated from sklearn):
 * SVM, SVR, XGB, XGR, Tree, Tree_regressor, KNN, KNN_regressor, NaiveBayes, GMM
   and the following ANNs
 * MLP, CNN (tbd)
 
 Here's [an animation that shows the progress of classification done with nkululeko](https://youtu.be/6Y0M382GjvM)
@@ -160,15 +161,16 @@
 * use a generic main python file (like my_experiment.py), 
 * adapt the path to your nkululeko src 
 * and then adapt an .ini file (again fitting at least the paths to src and data)
   
 Here's [an overview of the ini-file options](./ini_file.md)
 
 ### <a name="helloworld">Hello World example</a>
-* NEW: [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
+* NEW: [Here's a Google colab that runs this example out-of-the-box](https://colab.research.google.com/drive/1GYNBd5cdZQ1QC3Jm58qoeMaJg3UuPhjw?usp=sharing#scrollTo=4G_SjuF9xeQf), and here is the same [with Kaggle](https://www.kaggle.com/felixburk/nkululeko-hello-world-example)
+* [I made a video to show you how to do this on Windows](https://www.youtube.com/playlist?list=PLRceVavtxLg0y2jiLmpnUfiMtfvkK912D)
 * Set up Python on your computer, version >= 3.6
 * Open a terminal/commandline/console window
 * Test python by typing ```python```, python should start with version >3 (NOT 2!). You can leave the Python Interpreter by typing *exit()*
 * Create a folder on your computer for this example, let's call it `nkulu_work`
 * Get a copy of the [Berlin emodb in audformat](https://tubcloud.tu-berlin.de/s/LfkysdXJfiobiEG) and unpack the same folder (`nkulu_work`)
 * Make sure the folder is called "emodb" and does contain the database files directly (not box-in-a-box)
 * Also, in the `nkulu_work` folder: 
@@ -208,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.47.1
+--------------
+* enabled feature storage format csv for opensmile features
+
 Version 0.47.0
 --------------
 * added praat speech rate features
 
 Version 0.46.0
 --------------
 * added warnings for non-existent parameters
```

### Comparing `nkululeko-0.47.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.47.1/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.0/setup.cfg` & `nkululeko-0.47.1/setup.cfg`

 * *Files identical despite different names*

